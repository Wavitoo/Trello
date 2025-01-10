# Remake de Trello avec React, Node.js et MongoDB

# Table of Contents

1. [Description](#description)
2. [Fonctionnalités](#fonctionnalités)
   - [Dashboard](#dashboard)
   - [Gestion des Sections](#gestion-des-sections)
   - [Gestion des Tâches](#gestion-des-tâches)
3. [Prérequis](#prérequis)
4. [Installation](#installation)
   - [1. Clonez le repository](#1-clonez-le-repository)
   - [2. Installer les dépendances](#2-installer-les-dépendances)
   - [3. Configuration de la base de données](#3-configuration-de-la-base-de-données)
   - [4. Lancer l'application](#4-lancer-lapplication)
   - [5. Accéder à l'application](#5-accéder-à-lapplication)
5. [License](#license)
6. [Contributor](#contributor)

## Description

Ce projet est un remake de l'application Trello, avec un système de gestion de tâches, de tableaux et de sections. L'utilisateur peut se connecter, créer des tableaux, ajouter des sections, organiser des tâches et personnaliser l'interface de manière flexible. Le projet utilise React pour le frontend, **Node.js** et **Express** pour le backend, et **MongoDB** pour la gestion des données.

![dashboard](https://github.com/user-attachments/assets/38409020-d3a9-40bc-aac3-062d9f097758)

## Fonctionnalités

### Dashboard

- **Authentification** : Connexion et déconnexion de l'utilisateur.
- **Tableaux** : Les tableaux sont affichés en fonction de leur statut (favoris ou privés).
- **Tableaux favoris** : Les utilisateurs peuvent marquer certains tableaux comme favoris pour un accès rapide.
- **Tableaux privés** : Les tableaux privés sont visibles uniquement pour l'utilisateur connecté.
- **Options de tableau** : Le titre et la description des tableaux sont modifiables, et il est possible de supprimer un tableau via un bouton.

### Gestion des Sections

- **Ajout de sections** : Chaque tableau peut contenir plusieurs sections (par exemple, "À faire", "En cours", "Terminé").
- **Modification des sections** : Le titre des sections peut être modifié, et elles peuvent être supprimées.

![section](https://github.com/user-attachments/assets/a756eafe-8648-425c-8abc-954c99be104c)

### Gestion des Tâches

- **Création de cartes** : Chaque section peut contenir plusieurs tâches, sous forme de cartes.
- **Personnalisation des cartes** : Le contenu des cartes peut être modifié en utilisant plusieurs options de formatage :
    - Mise en forme du texte** : gras, italique, titres (H1, H2, H3, paragraphes).
    - Insertion de liens, listes (à puces ou numérotées), images et citations.
    - Gestion de l'indentation du texte.
    - Insertion de tableaux et autres médias.
- **Annuler/Rétablir** : Vous pouvez revenir en arrière ou refaire des actions précédentes.
- **Suppression des cartes** : Chaque carte peut être supprimée via un bouton.

## Prérequis

- Node.js et npm (ou yarn) installés sur votre machine.
- MongoDB (en local ou MongoDB Atlas pour une solution cloud).
- Un éditeur de texte comme Visual Studio Code.

## Installation

### 1. Clonez le repository

```bash
git clone git@github.com:Wavitoo/Trello.git
cd Trello
```
### 2. Installer les dépendances

**Backend (Node.js et Express)**

Dans le dossier `server` :

```bash
cd server
yarn install
```

**Frontend (React)**

Dans le dossier `client` :

```bash
cd client
yarn install
```

### 3. Configuration de la base de données

Assurez-vous que vous avez une base de données MongoDB opérationnelle. Si vous utilisez MongoDB Atlas, créez un cluster et obtenez l'URL de connexion. Ajoutez cette URL dans un fichier .env à la racine du dossier server.

Exemple de fichier .env :

```bash
PORT=
MONGODB_URL=mongodb://127.0.0.1:27017/nom_de_votre_db
PASSWORD_SECRET_KEY=
TOKEN_SECRET_KEY=
```

### 4. Lancer l'application

**Démarrer le serveur backend**

Dans le dossier `server` :

```bash
yarn start
```

Cela va lancer le serveur sur le port 3000 (par défaut) ou celui de votre fichier .env si vous avez renseigné un port.

**Démarrer le frontend**

Dans le dossier `client` :

```bash
yarn start
```

### 5. Accéder à l'application

Ouvrez votre navigateur et allez à http://localhost:3000 pour accéder à l'application.

## License

Ce projet est sous la licence MIT. Voir le fichier [LICENSE](https://github.com/Wavitoo/Trello/License) pour plus d'informations.

## Contributor

Ce projet a été réalisé par **Arslan TETU**.  
Si vous souhaitez me contacter, vous pouvez m'envoyer un email à [arslan.tetu@epitech.eu](mailto:arslan.tetu@epitech.eu).