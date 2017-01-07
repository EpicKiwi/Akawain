![Icon](resources/img/Akawain.svg)

# Akawain
> Un logiciel des gestion des vins en C# avec .Net

## Cahier des charges

* Logiciel compatible Windows en C# et .Net
* Archithecture MVC
* Utilisation des bibliothèques externes pour modulariser le logiciel
* Interface graphique Windows Form responsive
* Chargement des informations depuis une BDD
  * Choix de la base de données
  * BONUS : Pouvoir choisir entre plusieurs types de bases
  * Utiliser ADO.Net
  * Utiliser le pattern DAO
* BONUS : Système d'installation au premier démarrage
  * Configuration de l'acces à la base de données
  * Création automatique des tables

### Archithecture des données

Les données se présente comme ceci : 

#### Utilisateur

* id int auto-inc primary
* firstname varchar-255
* lastname varchar-255
* email varchar-255

#### Producteur

* id int auto-inc primary
* name varchar-255
* location varchar-255

#### Vin

* id int auto-inc primary
* owner foreign->Utilisateur.id
* area set(bordeaux;bourgogne)
* designation varchar-255
* type set(white;red;rose)
* producer foreign->Producteur.id
* millesime int
* quantity int
* grvariety varchar-255
* comment text
* BONUS : image varchar(255)

### Archithecture logicielle (WIP)

* Model
* View
  * Main window
  * Wine window
  * Profile window
  * BONUS : Install window
* Controller


## Crédits

* Icone raisins par [Freepik](http://www.flaticon.com/authors/freepik)
* Arrière plan d'icone par [Daniel Foré](http://danrabbit.deviantart.com/)
