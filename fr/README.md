# Isogeo Manager {#homepage}

Isogeo Manager appelée aussi "Manage" est une application interne qui permet d'effectuer des opérations dans la base de donnée d'Isogeo via l'API.

L'application Manager permet de gérer principalement :

* Les [mots-clés](/keywords/keywords.md) de la base centralisée ;
* Les [applications](/applications/list.md) autorisées à dialoguer avec l'API ;
* Les [groupes de travail](/groups/list.md) de la plateforme.

Seuls les utilisateurs de type *Staff* ont accès à l'application. Ils doivent [s'authentifier](https://id.api.isogeo.com/login?ReturnUrl=https%3A%2F%2Fid.api.isogeo.com%2Foauth%2Fauthorize%3Fresponse_type%3Dcode%26redirect_uri%3Dhttps%3A%252F%252Fmanage.isogeo.com%252Flogin%252Fcallback%26client_id%3Disogeo-manager) via la fenêtre d'authentification ci-dessous.

!["Fenêtre d'authentification"](/assets/authentication.png)

## Vision de l'application Manager  {#vision}

* **Pour** les gestionnaires de comptes Isogeo (équipe projet, équipe commerciale)
* **Qui** veulent administrer les groupes de travail et les utilisateurs de la plateforme Isogeo
* **Est** une application qui permet de gérer les comptes de la plateforme Isogeo : création, renommage ou suppression de groupes de travail, invitation d’utilisateurs... Elle permet l’activation ou la désactivation dynamique d’options gratuites ou payantes pour les groupes de travail.

## Déploiement {#deployments}

En mode *SaaS*, l'application est déployée sur des Web App Azure :

* QA : <https://qa-isogeo-manage.azurewebsites.net/>
* PROD : <https://manage.isogeo.com/>

## Version {#versions}

La version de l'application est indiquée à l'adresse <https://manage.isogeo.com/about> ou en bas à droite de la page.

!["Version de l'application"](assets/manager_version.png)

---

Date de la dernière mise à jour de cette documentation : {{ gitbook.time | date("DD/MM/YYYY") }}.
