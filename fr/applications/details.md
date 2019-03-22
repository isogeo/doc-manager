---
description: Gestion des applications de la base de données Isogeo dans l'application Isogeo Manager.
---

# Gérer une application {#manage_application}

Une application est un logiciel qui exploite l'API Isogeo. Il peut s'agir d'une application web (ex : APP), d'un logiciel bureautique (ex : Isogeo2office), d'un plugin (ex : plugin QGIS) ou simplement d'un script que l'on veut authentifier à l'API. En effet, c'est **ici que l'on récupère les clés d'accès à l'API**.

Pour plus d'informations sur les applications et l'API, veuillez consulter la page [précédente](list.md) et l'aide en ligne de l'[API](http://help.isogeo.com/api/fr/authentication/concepts.html).

## En-tête {#heading_application}

Dans l'en-tête, on retrouve plusieurs éléments.

!["En-tête de la présentation d'une application"](/assets/groups_heading.png)

### Nom de l'application {#application_name}

Le nom est modifiable dans le bloc [Détails](#application_names).

### Editer l'application (uniquement pour les applications de type utilisateur) {#edit_application}

Pour éditer les paramètres d'une application de type utilisateur, il faut cliquer sur l'icône <i class="fa fa-edit"></i> puis entrer le mot `EDIT` et valider.

Les applications utilisateurs comme *APP* ou le *scan FME* sont **sensibles**. Seul un développeur de ces applications est en capacité d'en modifier leurs paramètres.

### Supprimer l'application {#delete_application}

Pour supprimer l'application, il suffit de cliquer sur la poubelle <i class="fa fa-trash"></i> puis d'écrire en toute lettre `DELETE` et enfin supprimer.

!["Supprimer l'application"](/assets/applications_delete_application.png)

### Dates {#application_dates}

* La date de création correspond comme son nom l'indique à la date de création de l'application.

* La date de modification correspond à la date de dernière modification de l'un des paramètres de l'application. Soit tous ceux que nous allons découvrir dans la suite de cette documentation.

## Détails {#application_details}

Le bloc `Détails` permet de renseigner ou d'obtenir des informations sur l'application.

!["Détails d'une application](/assets/applications_details.png)

### Nom {#application_names}

Le nom de l'application est modifiable ici.

### Type d'application {#application_type}

On retrouve le type d'application sélectionné au moment de sa création.

### Droits (scopes) {#application_rights}

Il s'agit des droits de l'application sur l'API.

* resources:read (droits de lecture des ressources)
* groups:read (droits de lecture des groupes de travail)
* api:read (API en lecture complète)
* api:write (API en écriture complète)

### URL de base {#application_url}

Il s'agit de l'url de l'application. Si cet url n'est pas disponible, on peut mettre le lien vers l'aide en ligne de l'application.

### Options (uniquement pour les applications de type groupe) {#application_options}

En cochant la case `Peut être associée à plusieurs groupes`, il sera possible d'[associer](#associate_group) l'application à plusieurs groupes de travail.

Sinon, un message d'erreur s'affichera.

## Authentification {#application_authentication}

L'authentification à l'API utilise le protocole [OAuth 2.0](https://fr.wikipedia.org/wiki/OAuth) basé sur un couple d'identifiants clients *id/secret*.

!["Authentification de l'application"](/assets/applications_authentication.png)

### Copier dans le presse papier {#application_authentication_copy}

En cliquant sur *Copier dans le presse papier*, "coller" renvoit les informations d'authentification sous cette forme :

```
Demo Manager
Client ID: demo-manager-XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
Client Secret: XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
```

### Télécharger les paramètres au format JSON {#application_authentication_json}

Dans la plupart des applications existantes à Isogeo, il est possible d'authentifier ces-dernières en important le fichier *client_secrets.json* téléchargeable ici.

Le fichier JSON téléchargé contient ces informations sur l'application :

```json
{
    "web": {
        "client_id": "demo-manager-XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX",
        "client_secret": "XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX",
        "redirect_uris": [],
        "scopes": [
            "resources:read"
        ],
        "auth_uri": "https://id.api.isogeo.com/oauth/authorize",
        "token_uri": "https://id.api.isogeo.com/oauth/token"
    }
}
```

### Re-générer {#application_authentication_regenerate}

Cette fonctionnalité permet de re-générer les clients ID et Secret. 
Attention, comme l'indique le message de confirmation ci-dessous que doit valider l'utilisateur pour re-générer les identifiants ; il faudra diffuser les nouveaux identifiants aux developpeur de l'application pour qu'il puisse continuer à utiliser l'API.

!["Re-générer l’identifiant et le secret"](/assets/applications_authentication_regenerate.png)

Cette fonctionnalité permet d'avoir la main sur les développements autour de l'API. On peut choisir de révoquer à tout moment l'accès à l'API à un developpeur en re-générant ses clés.

## Groupes associés (uniquement pour les applications de type groupe) {#group_associated}

!["Partage d'un catalogue à une application depuis APP"](/assets/app_share_catalog_to_application.png)

Pour les applications de type groupe, il est possible d'associer des groupes de travail à l'application.

Cette association permet aux groupes de travail associés de partager des catalogues de métadonnées à l'application via le menu `Partages` sur APP.

!["Groupes associés"](/assets/applications_group_associated.png)

### Associer un groupe {#associate_group}

Pour associer un groupe,  il suffit de cliquer sur le bouton `Associer`, puis rechercher le groupe souhaité et cliquer dessus.

!["Associer un groupe"](/assets/applications_associate_group.png)

Le groupe apparait ensuite dans la liste des groupes associés. En cliquant sur `Voir le groupe`, le navigateur ouvre la page du groupe concerné sur le Manager.

Il est également possible de supprimer l'association au groupe via la poubelle <i class="fa fa-trash"></i>.

> Attention, si un utilisateur essaye d'associer un deuxième groupe à l'application et que la [case](#application_options) `Peut être associée à plusieurs groupes` n'est pas cochée, le message ci-dessous s'affiche.

!["Message d'erreur de l'association"](/assets/application_association_error.png)

## URLs de redirection (uniquement pour les applications de type utilisateur)

* Voir l'aide en ligne de l'[API](http://help.isogeo.com/api/fr/authentication/usersapps/userappuris.html)

## Type de sécurité (uniquement pour les applications de type utilisateur)

* Confidentielle : Une application confidentielle est capable de maintenir la confidentialité de ses identifiants. Une application web par exemple.
* Publique : Une application publique est incapable de maintenir la confidentialité de ses identifiants. Une application de navigateur (en JavaScript typiquement) par exemple.