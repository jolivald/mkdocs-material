# Utilisation de GitHub et VS Code

## Introduction

Ce cours vous guidera à travers les étapes de base pour utiliser GitHub et Visual Studio Code (VS Code) dans votre workflow de développement. Nous nous concentrerons sur les opérations fondamentales : ajouter des fichiers (add), valider des changements (commit), et pousser ces changements vers GitHub (push).

## Prérequis

- Installer [Git](https://git-scm.com/downloads) sur votre ordinateur
- Installer [Visual Studio Code](https://code.visualstudio.com/download)
- Créer un compte [GitHub](https://github.com/)
- Configurer Git avec vos informations GitHub  

```
git config --global user.name "VOTRE_NOM"
git config --global user.email "VOTRE_ADRESSE@mail.com"
```


## Création et clonage d'un dépôt

Sur GitHub :

- Connectez-vous à votre compte GitHub
- Cliquez sur "New" pour créer un nouveau dépôt
- Donnez un nom à votre dépôt et initialisez-le

Sur votre ordinateur :

- Ouvrez VS Code
- Ouvrez un terminal dans VS Code (Terminal > New Terminal)
- Naviguez vers le dossier où vous voulez cloner le dépôt
- Clonez le dépôt avec la commande :

    git clone https://github.com/votre-nom-utilisateur/nom-du-depot.git

---
## Création et clonage d'un dépôt

Création d'un dépôt sur GitHub :

 - Connectez-vous à votre compte GitHub
 - Cliquez sur "New" pour créer un nouveau dépôt
 - Donnez un nom à votre dépôt et initialisez-le avec un README

Clonage du dépôt avec VS Code :  

Il existe deux méthodes principales pour cloner un dépôt dans VS Code :

1. Utilisation de la palette de commandes

    1. Ouvrez VS Code
    2. Appuyez sur Ctrl+Shift+P (Windows/Linux) ou Cmd+Shift+P (Mac) pour ouvrir la palette de commandes
    3. Tapez "Git: Clone" et sélectionnez cette option
    4. Collez l'URL du dépôt GitHub que vous souhaitez cloner
    5. Choisissez un dossier local où vous voulez cloner le dépôt
    6. Une fois le clonage terminé, VS Code vous proposera d'ouvrir le dépôt cloné

2. Utilisation du terminal intégré

    1. Ouvrez VS Code
    2. Ouvrez un terminal dans VS Code (Terminal > New Terminal)
    3. Naviguez vers le dossier où vous voulez cloner le dépôt en utilisant la commande cd
    4. Clonez le dépôt avec la commande :  
    `git clone https://github.com/votre-nom-utilisateur/nom-du-depot.git`
    5. Ouvrez le dossier cloné dans VS Code (File > Open Folder)

## Obtenir l'URL du dépôt GitHub :

 - Sur la page de votre dépôt GitHub, cliquez sur le bouton vert "Code"
 - Copiez l'URL HTTPS affichée

## Note importante :

Après avoir cloné le dépôt, assurez-vous d'être dans le bon dossier pour les opérations suivantes.  
Si vous avez utilisé la méthode de la palette de commandes, VS Code vous placera automatiquement dans le bon dossier. Si vous avez utilisé la méthode du terminal, n'oubliez pas de naviguer dans le dossier cloné avec la commande `cd nom-du-depot`.

## Travailler avec VS Code

Dans VS Code, ouvrez le dossier du dépôt cloné (File > Open Folder)
Créez ou modifiez des fichiers dans ce dossier


## Ajouter des fichiers (add)

Lorsque vous avez créé ou modifié des fichiers :

 * Dans VS Code, allez dans l'onglet "Source Control" (Ctrl+Shift+G)
 * Vous verrez la liste des fichiers modifiés
 * Pour ajouter un fichier spécifique, cliquez sur le "+" à côté du nom du fichier
 * Pour ajouter tous les fichiers modifiés, cliquez sur le "+" à côté de "Changes"

Alternativement, vous pouvez utiliser le terminal intégré :

    git add nom-du-fichier

ou pour tous les fichiers :

    git add .


## Valider les changements (commit)

Après avoir ajouté vos fichiers :

 * Toujours dans l'onglet "Source Control", entrez un message de commit dans la zone de texte en haut
 * Cliquez sur le bouton "✓" (Commit) au-dessus de la zone de texte

Ou via le terminal :

    git commit -m "Votre message de commit"


## Pousser les changements vers GitHub (push)

Une fois vos changements validés localement :

 * Dans l'onglet "Source Control", cliquez sur les "..." (Plus d'actions)
 * Sélectionnez "Push"

Ou via le terminal :

    git push origin main

Note : main est généralement le nom de la branche principale, mais cela peut être master sur certains dépôts plus anciens.


## Bonnes pratiques

 * Commits fréquents : Faites des commits petits et fréquents plutôt que de grands commits peu fréquents
 * Messages de commit clairs : Écrivez des messages de [commit descriptifs](https://www.conventionalcommits.org/en/v1.0.0/) qui expliquent clairement les changements effectués
 * Pull avant Push : Avant de pousser vos changements, assurez-vous de récupérer les derniers changements du dépôt distant avec `git pull`
 * Vérifiez votre travail : Utilisez `git status` pour voir l'état de vos fichiers et `git log` pour voir l'historique des commits
