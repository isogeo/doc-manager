# Liste des applications

Cette page présente la liste de toutes les applications qui peuvent s'authentifier à l'API Isogeo.

## Types d'applications

Il existe deux types d'applications. Il est possible de filtrer sur l'un ou l'autre type en utilisant les boutons radios prévus à cet effet.

!["Filtrer selon le type d'application"](/assets/page_applications_radio_button.JPG)

### Groupe

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

NB : Pour les partenaires ou les clients qui developpent autour de l'API en lecture, des applications de type groupe sont également crées afin de leur générer des clés d'authentification.

### Utilisateur

Les applications de type utilisateur ne peuvent pas être associées à des groupes de travail. En effet, c'est l'utilisateur qui s'authentifie directement à l'application qui est elle-même authentifiée à l'API via ses clés.

Les principales applications de type utilisateurs existantes à Isogeo sont les suivantes :

* Isogeo App
* Isogeo Manager
* Isogeo Scan FME
* Python SDK

Isogeo Manager est donc une application de type utilisateur, c'est pour cette raison qu'il faut [s'authentifier](/fr/readme.md) avec son nom d'utilisateur et son mot de passe Isogeo.

## Rechercher une application

Il est possible de filtrer sur les applications contenant le nom recherché.

Par exemple : en tapant `plugin` (cf. figure ci-dessous), la liste s'adapte automatiquement et renvoit tous les applications dont le nom **contient** `plugin` par ordre alphabétique.

> NB : Il n'est pas nécéssaire de cliquer sur la touche `entrée` car la liste des mots-clés est filtrée automatiquement lorsque l'utilisateur écrit dans la barre de recherche.

!["Rechercher des applications"](/assets/page_applications_research_plugin.JPG)

## Pagination

Pour naviguer facilement dans la liste, un système de pagination permet de naviguer page par page en cliquant sur les simples flèches ou les numéros de page. Les doubles-flèches permettent elles d'accèder directement à la premiere ou la dernière page.

> NB : Lors d'une recherche ou d'un tri, le système de pagination s'adapte automatiquement en fonction de la liste.