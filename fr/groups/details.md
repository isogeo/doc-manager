---
description: Gestion des groupes de travail de la base de données Isogeo dans l'application Isogeo Manager.
---

# Gérer un groupe {#manage_group}

Le groupe de travail est au coeur du modèle d'Isogeo. Il correspondant à un entrepôt de fiche de métadonnées et possède ses propres paramètres d'administration. L'application Manager permet de gérer ses autorisations.

Plusieurs blocs permettent de gérer le groupe.

## En-tête {#heading}

Dans l'en-tête, on retrouve plusieurs éléments.

!["En-tête de la présentation d'un groupe"](/assets/groups_heading.png)

### Nom du groupe de travail {#group_name}

Le nom est modifiable dans le bloc [Coordonnées](#group_coordinates).

### Lien vers le groupe de travail sur la plateforme Isogeo {#link_group_app}

En cliquant sur APP<i class="fa fa-external-link"></i>, le navigateur ouvre le groupe de travail sur https://app.isogeo.com.

Si vous êtes déjà connecté sur un autre groupe de travail, le lien ne fonctionnera pas car votre navigateur forcera l'ouverture vers ce dernier.

Pour contourner :

1. Clic droit sur APP<i class="fa fa-external-link"></i> ;
2. Copier l'adresse du lien dans un éditeur de texte ;
3. Copier l'ID du groupe (ex : 628a29a84c354713a9ae14989e0fdd68) ;
4. Ouvrir https://app.isogeo.com ;
5. Coller l'ID dans l'url de la barre d'adresse à la place de l'ID de l'autre groupe.

!["Coller ici l'ID"](/assets/groups_copy_id_group.png)

### Supprimer le groupe {#delete_group}

Pour supprimer le groupe, il suffit de cliquer sur la poubelle <i class="fa fa-trash"></i> puis d'écrire en toute lettre `DELETE` et enfin supprimer.

!["Supprimer le groupe"](/assets/groups_delete_group.png)

### Dates {#group_dates}

* La date de création correspond comme son nom l'indique à la date de création du groupe de travail.

* La date de modification correspond à la date de dernière modification de l'un des paramètres du groupe. Soit tous ceux que nous allons découvrir dans la suite de cette documentation.

## Coordonnées {#group_coordinates}

Le bloc `Coordonnées` permet de renseigner des informations sur le groupe de travail. Ces informations peuvent être également modifiées par un administrateur du groupe de travail sur APP (cf. [Aide en ligne Admin](https://help.isogeo.com/admin/fr/settings/dashboard.html#le-point-de-contact-du-groupe-de-travail)).

!["Renseigner les coordonnées du groupe depuis l'application Manager"](/assets/groups_coordinates.png)

!["Renseigner les coordonnées du groupe depuis APP"](/assets/app_groups_coordinates.png)

## Modules {#group_modules}

Ici, il est possible d'activer des modules auxquels aura accès le groupe de travail dans APP. Ces activations s'effectuent en fonction de la commande des clients, l'offre Isogeo étant modularisée.

!["Modules d'un groupe"](/assets/groups_modules.png)

### Client CSW {#csw}

En activant le module, le groupe de travail aura accès au client CSW dans l'administration soit le menu `Synchronisation`.

!["Client CSW activé dans APP"](/assets/groups_activate_csw_app.png)

Sinon, le menu `Synchronisation` n'apparait pas.

### Scan FME {#scan}

En activant le module, le groupe de travail aura accès au Scan FME dans l'administration soit le menu `Scan FME`.

!["Scan FME activé dans APP"](/assets/groups_activate_scan_app.png)

Si le module est desactivé le message ci-dessous s'affiche.

!["Scan FME désactivé dans APP"](/assets/groups_desactivate_scan_app.png)

### Partage {#share}

En activant le module, le groupe de travail aura la possibilité de partager des catalogues de fiches de métadonnées à d'autres groupes de travail dans l'administration depuis le menu `Partages`.

!["Partage activé dans APP"](/assets/groups_activate_partage_app.png)

Si le module est désactivé, la création d'un partage vers un autre groupe de travail ne sera pas possible.
 
### Diffusion {#diffusion}

Ce module n'existe plus, laissez la case décochée.

## Ressources {#ressources}

Dans ce bloc, le fonctionnement est similaire à celui des modules. Il s'agit des limitations fixées au groupe de travail. Ces limitations sont également négociées lors de la vente.

!["Les ressources d'un groupe"](/assets/groups_ressources.png)

### Couleurs de la jauge {#gauge_color}

* <span style="color:#5cb85c">Vert : les limites ne sont pas atteintes.</span>
* <span style="color:#f0ad4e">Orange : les limites sont atteintes.</span>
* <span style="color:#d9534f">Rouge : les limites sont dépassées.</span>

### Ressources illimités {#unlimited}

L'offre commerciale d'Isogeo propose des packs de fiches et d'utilisateurs illimités. Pour rendre les ressources illimités, il faut sélectionner **-1** au niveau des curseurs concernés.

### Conséquences d'un dépassement de limites {#exceeding}

Lorsque les limites sont dépassées, les utilisateurs du groupe de travail verront le message ci-dessous à chaque ouverture d'APP.

Cependant, hormis cette fenêtre polluante à quitter à chaque fois, ils pourront toujours utiliser les fonctionnalités de la plateforme.  

!["Message alertant le depassement des limites dans APP"](/assets/app_limits_exceeded.png)

## Utilisateurs {#user_group}

Ce bloc liste tous les utilisateurs du groupe de travail avec leur rôle.

Le membre du staff Isogeo qui crée le groupe dans l'application Manager est **automatiquement** ajouté aux utilisateurs du groupe de travail.

Cette liste est également visible depuis la [page d'administration](https://app.isogeo.com/groups/628a29a84c354713a9ae14989e0fdd68/admin/users/memberships) du groupe de travail dans APP.

### Invitations {#invitation}

Il est possible d'inviter des utilisateurs dans le groupe de travail en cliquant sur le bouton `Inviter`. Ensuite, une fenêtre s'ouvre dans laquelle il faut renseigner l'adresse mail et le rôle souhaité puis valider.

L'invitation est valide pendant 7 jours. L'invité doit donc accepter l'invitation dans ses mails dans ce délais sous peine de recevoir un message d'erreur. Le temps restant avant l'expiration est indiqué dans l'invitation (cf. figure ci-dessous).

Pour supprimer une invitation, la poubelle <i class="fa fa-trash"></i> est prévue à cet effet. L'utilisateur recevra quand même le mail mais il ne pourra pas accéder au groupe de travail.

!["Les utilisateurs d'un groupe et les invitations ](/assets/groups_users.png)

## Applications {#group_associate_applications}

Il est possible d'associer des applications au groupe mais il faut au préalable [créer l'application](/fr/applications/create.md) dans l'application Manager.

Ensuite, il suffit de rechercher l'application souhaitée avec son nom parmi la liste des applications recensées.

!["Associer une application à un groupe"](/assets/groups_associate_application.png)

## Paramètres {#group_parameters}

Quelques paramètres peuvent encore être réglés depuis la page de gestion d'un groupe.

!["Réglages des paramètres d'un groupe depuis l'application Manager"](/assets/groups_parameters.png)

Ces paramètres sont également réglables depuis l'[administration](https://app.isogeo.com/groups/628a29a84c354713a9ae14989e0fdd68/admin/settings) d'APP.

!["Réglages des paramètres d'un groupe depuis APP"](/assets/app_parameters.png)

### Référencer le groupe dans les contacts {#allow_contact_group}

Le point de contact du groupe de travail correspond aux [coordonnées](#group_coordinates) renseignées précèdemment.

Ces contacts sont centralisés dans la base de données d'Isogeo et peuvent être visibles par les autres groupes de travail **si cette option est cochée**.

Cette visibilité se traduit par la possibilité d'ajouter le point de contact d'un autre groupe de travail dans ses fiches de métadonnées.  

Exemple : Dans la figure ci-dessous, j'ai ajouté Demo Manager en contact d'une fiche du groupe de travail Isogeo Tests.

!["Réglages des paramètres depuis APP"](/assets/app_association_contact_group.png)

### Autoriser la création de fiche manuelles {#allow_fiche_manually}

Lorsque cette case est cochée, l'utilisateur de type administrateur ou éditeur peut donc créer des fiches manuelles. Le bouton `Créer` apparait alors dans l'inventaire du groupe de travail sur APP. Sinon, le bouton n'apparait pas.

!["Création d'une fiche manuelle depuis APP](/assets/app_creation_md_manually.png)

### Autoriser la création manuelle de liens vers des services cartographiques (dépréciée)

Cette option est dépréciée, laissez la décochée.

### Langue des métadonnées {#group_md_language}

La langue d’une métadonnée doit être spécifiée dans l’onglet `Métadonnée` d’une fiche de métadonnées.

Pour que celle-ci soit renseignée automatiquement sur chaque nouvelle fiche de métadonnées créée, il suffit de choisir la langue parmi celles proposées.