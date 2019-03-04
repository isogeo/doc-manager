# Gérer un groupe

Le groupe de travail est au coeur du modèle d'Isogeo. Il correspondant à un entrepôt de fiche de métadonnées et possède ses propres paramètres d'administration. Le Manager permet de gérer ses autorisations.

Plusieurs blocs permettent de gérer le groupe.

## En-tête

Dans l'en-tête, on retrouve plusieurs éléments.

!["En-tête de la présentation d'un groupe"](/assets/groups_heading.JPG)

### Nom du groupe de travail

Le nom est modifiable dans le bloc [Coordonnées](#coordonnées).

### Lien vers le groupe de travail sur la plateforme Isogeo

En cliquant sur APP<i class="fa fa-external-link"></i>, le navigateur ouvre le groupe de travail sur https://app.isogeo.com.

Si vous êtes déjà connecté sur un autre groupe de travail, le lien ne fonctionnera pas car votre navigateur forcera l'ouverture vers ce dernier.

Pour contourner :

1. Clic droit sur APP<i class="fa fa-external-link"></i> ;
2. Copier l'adresse du lien dans un éditeur de texte ;
3. Copier l'ID du groupe (ex : 628a29a84c354713a9ae14989e0fdd68) ;
4. Ouvrir https://app.isogeo.com ;
5. Coller l'ID dans l'url de la barre d'adresse à la place de l'ID de l'autre groupe.

!["Coller ici l'ID"](/assets/groups_copy_id_group.JPG)

### Supprimer le groupe

Pour supprimer le groupe, il suffit de cliquer sur la poubelle <i class="fa fa-trash"></i> puis d'écrire en toute lettre `DELETE` et enfin supprimer.

!["Supprimer le groupe"](/assets/groups_delete_group.JPG)

### Dates

* La date de création correspond comme son nom l'indique à la date de création du groupe de travail.

* La date de modification correspond à la date de dernière modification de l'un des paramètres du groupe. Soit tous ceux que nous allons découvrir dans la suite de cette documentation.

## Coordonnées

Le bloc `Coordonnées` permet de renseigner des informations sur le groupe de travail. Ces informations peuvent être également modifiées par un administrateur du groupe de travail sur APP (cf. [Aide en ligne Admin](http://help.isogeo.com/admin/fr/settings/dashboard.html#le-point-de-contact-du-groupe-de-travail)).

!["Renseigner les coordonnées du groupe depuis Manager"](/assets/groups_coordinates.JPG)

!["Renseigner les coordonnées du groupe depuis APP"](/assets/app_groups_coordinates.JPG)

## Modules

Ici, il est possible d'activer des modules auxquels aura accès le groupe de travail dans APP. Ces activations s'effectuent en fonction de la commande des clients, l'offre Isogeo étant modularisée.

!["Modules d'un groupe"](/assets/groups_modules.JPG)

### Client CSW

En activant le module, le groupe de travail aura accès au client CSW dans l'administration soit le menu `Synchronisation`.

!["Client CSW activé dans APP"](/assets/groups_activate_csw_app.JPG)

Sinon, le menu `Synchronisation` n'apparait pas.

### Scan FME

En activant le module, le groupe de travail aura accès au Scan FME dans l'administration soit le menu `Scan FME`.

!["Scan FME activé dans APP"](/assets/groups_activate_scan_app.JPG)

Si le module est desactivé le message ci-dessous s'affiche.

!["Scan FME désactivé dans APP"](/assets/groups_desactivate_scan_app.JPG)

### Partage

En activant le module, le groupe de travail aura la possibilité de partager des catalogues de fiches de métadonnées à d'autres groupes de travail dans l'administration depuis le menu `Partages`.

!["Partage activé dans APP"](/assets/groups_activate_partage_app.JPG)

Si le module est désactivé 

* TO DO 

### Diffusion

Ce module n'existe plus, laisser la case décochée.

## Ressources

Dans ce bloc, le fonctionnement est similaire à celui des modules. Il s'agit des limitations fixées au groupe de travail. Ces limitations sont également négociées lors de la vente.

!["Les ressources d'un groupe"](/assets/groups_ressources.JPG)

### Couleurs de la jauge

* <span style="color:#5cb85c">Vert : les limites ne sont pas atteintes</span>
* <span style="color:#f0ad4e">Orange : les limites sont atteintes</span>
* <span style="color:#d9534f">Rouge : les limites sont dépassées</span>

Rastafari !

### Ressources illimités

L'offre commerciale d'Isogeo propose des packs de fiches et d'utilisateurs illimités. Pour rendre les ressources illimités, il faut sélectionner **-1** au niveau des curseurs concernés.

### Conséquences d'un dépassement de limites

Lorsque les limites sont dépassées, les utilisateurs du groupe de travail verront le message ci-dessous à chaque ouverture d'APP.

Cependant, hormis cette fenêtre polluante à quitter à chaque fois, ils pourront toujours utiliser les fonctionnalités de la plateforme.  

!["Message alertant le depassement des limites dans APP"](/assets/app_limits_exceeded.JPG)

## Utilisateurs

Ce bloc liste tous les utilisateurs du groupe de travail avec leur rôle.

Le membre du staff Isogeo qui crée le groupe dans Manager est **automatiquement** ajouté aux utilisateurs du groupe de travail.

Cette liste est également visible depuis la [page d'administration](https://app.isogeo.com/groups/628a29a84c354713a9ae14989e0fdd68/admin/users/memberships) du groupe de travail dans APP.

### Invitations

Il est possible d'inviter des utilisateurs dans le groupe de travail en cliquant sur le bouton `Inviter`. Ensuite, une fenêtre s'ouvre dans laquelle il faut renseigner l'adresse mail et le rôle souhaité puis valider.

L'invitation est valide pendant 7 jours. L'invité doit donc accepter l'invitation dans ses mails dans ce délais sous peine de recevoir un message d'erreur. Le temps restant avant l'expiration est indiqué dans l'invitation.

Pour supprimer une invitation, la poubelle est prévue à cet effet. L'utilisateur recevra quand même le mail mais il ne pourra pas accéder au groupe de travail.

!["Les utilisateurs d'un groupe et les invitations ](/assets/groups_users.JPG)

## Applications

Il est possible d'associer des applications au groupe mais il faut au préalable [créer l'application](/fr/applications/details.md) dans le Manager.

Ensuite, il suffit de rechercher l'application souhaitée avec son nom parmi la liste des applications recensées.

!["Associer une application à un groupe"](/assets/groups_associate_application.JPG)

> NB : Cette fonctionnalité ne fonctionne pas actuellement. Le bug est déclaré sur [Github](https://github.com/isogeo/isogeo-manager/issues/9).

## Paramètres

### Référencer le groupe dans les contacts

### Autoriser la créeation de fiche manuelles

### Autoriser la création manuelle de liens vers des services cartographiques 

### Langue des métadonnées


!["Paramètres d'un groupe"](/assets/groups_parameters.JPG)