# Gérer un groupe

Le groupe de travail est au coeur du modèle d'Isogeo. Il correspondant à un entrepôt de fiche de métadonnées et possède ses propres paramètres d'administration. Le Manager permet de gérer ses autorisations.

## Créer un groupe

Pour créer un groupe, il suffit de cliquer sur `Groupe` puis `Ajouter un groupe` et renseigner son nom avant de valider.

!["Ajouter un groupe"](/assets/groups_add_group.JPG)

## Paramétrage

Plusieurs blocs permettent de gérer le groupes. 

### En-tête

Dans l'en-tête, on retrouve plusieurs éléments.

!["En-tête de la présentation d'un groupe"](/assets/groups_heading.JPG)

#### Nom du groupe de travail

Le nom est modifiable dans le bloc [Coordonnées](#Coordonnées)

#### Lien vers le groupe de travail sur la plateforme Isogeo

En cliquant sur APP<i class="fa fa-external-link"></i>, le navigateur ouvre le groupe de travail sur https://app.isogeo.com.

Si vous êtes déjà connecté sur un autre groupe de travail, le lien ne fonctionnera pas car votre navigateur forcera l'ouverture vers ce dernier.

Pour contourner :

1. Clic droit sur APP<i class="fa fa-external-link"></i>
2. Copier l'adresse du lien dans un éditeur de texte
3. Copier l'ID du groupe (ex : 628a29a84c354713a9ae14989e0fdd68)
4. Ouvrir https://app.isogeo.com
5. Coller l'ID dans l'url de la barre d'adresse à la place de l'ID de l'autre groupe

!["Coller ici l'ID"](/assets/groups_copy_id_group.JPG)

#### Supprimer le groupe

Pour supprimer le groupe, il suffit de cliquer sur la poubelle <i class="fa fa-trash"></i> puis d'écrire en toute lettre `DELETE` et enfin supprimer.

!["Supprimer le groupe"](/assets/groups_delete_group.JPG)

#### Dates

La date de création correspondant comme son nom l'indique à la date de création du groupe de travail.

La date de modification correspond à la date de dernière modification de l'un des paramètres du groupe. Soit tous ceux que l'on allons découvrir dans la suite de cette documentation.

### Coordonnées

Le bloc `Coordonnées` permet de renseigner des informations sur le groupe de travail. Ces informations peuvent être également modifiées par un adminsitrateur du groupe de travail sur APP (cf. [Aide en ligne Admin](http://help.isogeo.com/admin/fr/settings/dashboard.html#le-point-de-contact-du-groupe-de-travail)).

!["Renseigner les coordonnées du groupe depuis Manager"](/assets/groups_coordinates.JPG)

!["Renseigner les coordonnées du groupe depuis APP"](/assets/app_groups_coordinates.JPG)

### Modules

Ici, il est possible d'activer des modules auxquels aura accès le groupe de travail dans APP. Ces activations s'effectuent en fonction de la commande des clients, l'offre Isogeo étant modularisée.

!["Modules d'un groupe"](/assets/groups_modules.JPG)

#### Client CSW

En activant le module, le groupe de travail aura accès au client CSW dans l'administration soit le menu `Synchronisation`.

!["Client CSW activé dans APP"](/assets/groups_activate_csw_app.JPG)

Sinon, le menu `Synchronisation` n'apparait pas.

#### Scan FME

En activant le module, le groupe de travail aura accès au Scan FME dans l'administration soit le menu `Scan FME`.

!["Scan FME activé dans APP"](/assets/groups_activate_scan_app.JPG)

Si le module est desactivé le message ci-dessous s'affiche.

!["Scan FME désactivé dans APP"](/assets/groups_desactivate_scan_app.JPG)

#### Partage

En activant le module, le groupe de travail aura la possibilité de partager des catalogues de fiches de métadonnées à d'autres groupes de travail dans l'administration depuis le menu `Partages`.

!["Partage activé dans APP"](/assets/groups_activate_csw_app.JPG)

Si le module est désactivé 

* TO DO 

#### Diffusion

Ce module n'existe plus, laisser la case décochée.

### Ressources

Dans ce bloc, le fonctionnement est similaire à celui des modules. Il s'agit des limitations fixées au groupe de travail. Ces limitations sont également négociées lors de la vente. L'offre commerciale d'Isogeo propose des packs de fiches et d'utilisateurs illimités. Pour rendre les ressources illimités, il faut sélectionner **-1** au niveau des curseurs concernés.

#### Fiches

#### Catalogues

#### Utilisateurs

#### Stockage

### Utilisateurs

Ce bloc liste tous les utilisateurs du groupe de travail.




### Applications

### Paramètres
