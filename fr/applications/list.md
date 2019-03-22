---
description: Lister les applications de la base de données Isogeo dans l'application Isogeo Manager.
---

# Liste des applications {#list_application}

Cette page présente dans l'ordre alphabétique la liste de toutes les applications qui peuvent s'authentifier à l'API Isogeo.

## Types d'applications {#type_application}

Il existe deux types d'applications. Il est possible de filtrer sur l'un ou l'autre type en utilisant les boutons radios prévus à cet effet.

!["Filtrer selon le type d'application"](/assets/applications_radio_button.png)

### Applications de groupe {#group_type}

Les applications de type groupe peuvent être associées à un ou plusieurs groupes de travail. En effet, c'est le groupe de travail qui s'authentifie à l'application qui est elle-même authentifiée à l'API via ses clés.

Les principales applications de type groupe existantes à Isogeo sont les suivantes :

* CSW
* OpenCatalog
* Carthothèque
* Extracteur FME
* Portail de données
* Isogeo2Office
* Plugin QGIS
* Plugin ArcMap
* Widget WebAppBuilder

> NB : Pour les partenaires ou les clients qui développent autour de l'API en lecture, des applications de type groupe sont également crées afin de leur générer des clés d'authentification.

### Applications utilisateur {#user_type}

Les applications de type utilisateur ne peuvent pas être associées à des groupes de travail. En effet, c'est l'utilisateur qui s'authentifie directement à l'application qui est elle-même authentifiée à l'API via ses clés.

Les principales applications de type utilisateurs existantes à Isogeo sont les suivantes :

* Isogeo App
* Isogeo Manager
* Isogeo Scan FME
* Python SDK

L'application Manager est donc une application de type utilisateur, c'est pour cette raison qu'il faut s'authentifier avec son nom d'utilisateur et son mot de passe Isogeo.

> Pour plus d'informations sur les types d'application, veuillez consulter l'aide en ligne de l'[API](http://help.isogeo.com/api/fr/authentication/concepts.html).

## Rechercher une application {#research_application}

Il est possible de filtrer sur les applications contenant le nom recherché.

Par exemple : en tapant `plugin` (cf. figure ci-dessous), la liste s'adapte automatiquement et renvoit tous les applications dont le nom **contient** `plugin` par ordre alphabétique.

> NB : Il n'est pas nécéssaire de cliquer sur la touche `entrée` car la liste des mots-clés est filtrée automatiquement lorsque l'utilisateur écrit dans la barre de recherche.

!["Rechercher des applications"](/assets/applications_research_plugin.png)

## Modification d'une application {#modify_application}

Pour modifier les paramètres d'une application, il suffit de cliquer sur l'application concernée dans la liste et la page de présentation de l'application s'affiche. Pour plus d'informations sur le paramètrage des différents blocs, veuillez consulter la [page suivante](details.md).

## Pagination {#pagination_application}

Pour naviguer facilement dans la liste, un système de pagination permet de naviguer page par page en cliquant sur les simples flèches ou les numéros de page. Les doubles-flèches permettent elles d'accèder directement à la première ou la dernière page.

> NB : Lors d'une recherche ou d'un tri, le système de pagination s'adapte automatiquement en fonction de la liste.