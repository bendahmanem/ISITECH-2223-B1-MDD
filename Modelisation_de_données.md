# Modelisation de donnees (Merise, MCD, MLD, MPD)

## 0. Informations sur la prise de notes et la notation

- Les notes sont prises en Markdown
- Tout rendu se fait avec un depot Git
- La qualite de la prise de note fera partie de la note finale

- Au cours de l'examen l'utilisation ou toute suspicion d'utilisation de chat GPT entrainera une note de 0

## 1. Introduction a Git

Pour creer un depot Git, placez vous au sein d'un repertoire et entrez la commande :

```sh
git init
```

Cette commande va initialiser un depot Git, Git va traquer les toutes les modifications effectuées au sein de ce dossier.

Pour consulter l'etat du depot Git il suffit de lancer la commande :

```bash
git status
```

Pour ajouter des fichiers non suivis :

```bash
git add .
```

Pour sauvegarder votre travail :

```bash
git commit -m "votre message de commit"
```

## 2. Merise

Merise est une méthode de modélisation de données. Elle permet de représenter les données d'un système d'information.
Merise est un acrnonyme de : Méthode d'Etude et de Réalisation Informatique pour les Systèmes d'Entreprise.

Presentation generale
Cette methode se caracterise par trois points clés:

- une approche dite systemique : on transforme les processus de l'entreprise en systeme d'information
- une separation des donnees et des traitements
- une approche nivelée

### L'approche systemique

![Alt text](image.png)

Le systeme de pilotage:

- Il est compose de l'ensemble des acteurs qui vont **piloter** le systeme d'information

Le systeme d'information:

- Il est compose de l'ensemble des acteurs qui vont **utiliser** le systeme d'information

Le systeme operant :

- Il est compose de l'ensemble des acteurs qui vont **produire** les donnees du systeme d'information

### La separation des donnees et des traitements

La separation des donnees et des traitements permet de separer les donnees du systeme d'information et les traitements effectues sur ces donnees.
Cette demarche se fait en 3 etapes :

- L'analyse des flux : on analyse les flux d'informations entre les acteurs du systeme d'information et les acteurs du systeme operant
- L'etude des documents internes (factures, bon de livraison,)
- L'etude des documents en externes (fournisseurs, clients,).

Les differents types d'informations:

- les infos de bases ou elementaires : ce sont les donnees de base du systeme d'information
- les informations calculees : ce sont les donnees calculees a partir des donnees de base
- les traitements ou les fonctions : ce sont les traitements effectues sur les donnees de base pour obtenir les donnees calculees

En résumé : vous devrez identifier les données et les traitements effectués sur ces données.

### L'approche nivelée

Pour effectuer la conception d'un SI, on va utiliser une approche nivelée. Cette approche se compose de 4 niveaux :

- le niveau conceptuel
- le niveau organisationnel
- le niveau logique
- le niveau physique

#### Le niveau conceptuel

Le niveau conceptuel permet de modéliser les données de l'entreprise. On va utiliser le modèle conceptuel de données (MCD) pour modéliser les données de l'entreprise, et le MCT pour modéliser les traitements effectués sur ces données.

#### Le niveau organisationnel

Le niveau organisationnel va permettre d'integrer a l'analyse precedente toutes les notions de temporalite, de chronologie des operations, de contraintes geographique, niveau d'acces. On va utiliser le modele organisationnel des traitements (MOT) et le modele organisationnel des donnees (MOD) pour modéliser les traitements de l'entreprise.

En resume on se pose les questions suivantes a partir des donnees recueillies au niveau conceptuel :

- **Quand** les traitements sont-ils effectues ?
- **Où** les traitements sont-ils effectues ?
- Par **qui** les traitements sont-ils effectues ?

#### Le niveau logique

Le niveau logique va permettre de modéliser les données de l'entreprise en utilisant le modèle logique de données (MLD) et les traitements de l'entreprise en utilisant le modèle logique des traitements (MLT).

Le MLD est independant des langages de programmation et des SGBD (Systeme de Gestion de Base de Donnees).

On repond a la question : **Avec Quoi** les traitements sont-ils effectues ?

#### Le niveau physique

Il s'agit de l'organisation `réelle` des données. On va utiliser le modèle physique de données (MPD) et le modèle physique des traitements (MPT).

Ici, on apporte les solutions techniques de stockage des données et de traitement des données.

On repond a la question : **Comment** les traitements sont-ils effectues ?

#### Résumé: les 4 niveau de Merise

![Alt text](image-1.png)
