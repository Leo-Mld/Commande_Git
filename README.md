# Commande-Git


Git config

Elle permet de configurer les préférences de l’utilisateur ( mail, nom d’utilisateur )
    
    git config --global user.name "name"
    git config --global user.email "email"


Git init

Permet d'Initialiser nouveau dépôt GIT :

    git init


Git add

Permet d'ajouter des fichiers à l’index.

    git add temp.txt


Clone git

Est utilisée pour cloner notre dépôt. 

    git clone git@github.com:name/namedepot


Create a new repository

    git clone git@gitlab.com:user/<ID>.git
    cd <ID>
    touch README.md
    git add README.md
    git commit -m "add README"
    git push -u origin master


Push an existing folder

    cd existing_folder
    git init
    git remote add origin git@gitlab.com:user/<ID>.git
    git add .
    git commit -m "Initial commit"
    git push -u origin master


Push an existing Git repository

    cd existing_repo
    git remote rename origin old-origin
    git remote add origin git@gitlab.com:user/<ID>.git
    git push -u origin --all
    git push -u origin --tags

Git commit

Permet de valider les modifications apportées.

    git commit –m “Description du commit”


Git status

Affiche la liste des fichiers modifiés ainsi que les fichiers qui doivent encore être ajoutés ou validés.

    git status


Git push

Envoie les modifications locales apportées à la branche associée.

    git push origin master


Git checkout

Permet de créer des branches. 

    git checkout -b <nom-branche>

Pour passer d’une branche à une autre.

    git checkout <nom-branche>


Git remote

Permet à l’utilisateur de connecter le dépôt local à un serveur distant:

    git remote add origin <93.188.160.58>


Branche git

Est être utilisée pour répertorier, créer ou supprimer des branches et our répertorier toutes les branches présentes dans le dépôt.

    git branch

Pour supprimer une branche.

    git branch –d <nom-branche>


Git pull

Pour fusionner toutes les modifications présentes sur le dépôt distant dans le répertoire de travail local.

    git pull


Git merge

Est utilisée pour fusionner une branche dans la branche active.

    git merge <nom-branche>


Git diff

Permet de lister les conflits.

    git diff --base <nom-fichier>

Pour afficher les conflits entre les branches à fusionner avant de les fusionner.

    git diff <branche-source> <branche-cible>

Pour  énumérer tous les conflits actuels.

    git diff


Git tag

Le marquage est utilisé pour marquer des commits spécifiques avec des poignées simples. 

    git tag 1.1.0 <insert-commitID-here>


Git log

Génère le log d’une branche. 

    commit 15f4b6c44b3c8344caasdac9e4be13246e21sadw 
    Author: Alex Hunter <alexh@gmail.com> 
    Date: Mon Oct 1 12:56:29 2016 -0600


Git reset

Pour réinitialiser l’index et le répertoire de travail à l’état du dernier commit.

    git reset --hard HEAD


Git rm

Est utilisé pour supprimer des fichiers de l’index et du répertoire de travail.

    git rm nomfichier.txt


Git stash

Permet d'enregistrer les changements qui ne doivent pas être commit immédiatement.

    git stash


Git show

Permet d'afficher des informations sur tout fichier git.

    git show


Git fetch

Permet à un utilisateur d’extraire tous les fichiers du dépôt distant qui ne sont pas actuellement dans le répertoire de travail local.

    git fetch origin


Git ls-tree

Pour afficher un fichier arborescent avec le nom et le mode de chaque élément et la valeur SHA-1 du blob, utilisez la commande git ls-tree. 

    git ls-tree HEAD


Git cat-file

À l’aide de la valeur SHA-1, affichez le type d’un fichier à l’aide de la commande git cat-file . 

    git cat-file –p d670460b4b4aece5915caf5c68d12f560a9fe3e4


Git grep

Permet à un utilisateur de rechercher dans les arbres de contenu des expressions et / ou des mots.

    git grep "www.hostinger.com"


Gitk

Gitk est l’interface graphique du dépôt local. 

    gitk


Git instaweb

Un serveur Web peut être exécuté par interface avec le dépôt local. Qui redirige directement vers un serveur web.

    git instaweb –httpd=webrick


Git gc

Pour optimiser le dépôt en supprimant les fichiers inutiles et les optimiser.

    git gc


git archive

Permet à un utilisateur de créer un fichier zip ou tar contenant les composants d’un arbre du dépôt. 

    git archive --format=tar master


Git prune

Via la commande git prune , les fichiers qui n’ont pas de pointeurs entrants seront supprimés. 

    git prune


Git fsck

Pour effectuer une vérification d’intégrité du système de fichiers git. Tous les fichiers corrompus seront identifiés.

    git fsck


Git rebase

Permet la réapplication des commits sur une autre branche.

    git rebase master
