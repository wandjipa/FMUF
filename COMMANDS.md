INSTALLER GIT
=============
GitHub est un outil de travail en ligne permettant de mettre en communs des modifications effectuées par plusieurs personnes sur un projet donné.

GitHub pour Windows: https://windows.github.com
GitHub pour Mac : https://mac.github.com
Git pour Linux - Solaris : http://git-scm.com

CONFIGURATION DES OUTILS
========================
Configurer les informations de l'utilisateur pour tous les dépôts locaux

**$ git config --global user.name "[nom]"**
Définit le nom que vous voulez associer à toutes vos opérations de commit

**$ git config --global user.email "[adresse email]"**
Définit l'email que vous voulez associer à toutes vos opérations de commit

**$ git config --global http.proxy http://192.168.1.17:8080**
Définit le proxy de l’école à utiliser

**$ git config --global –unset http.proxy**
Réinitialise la valeur du proxy à utiliser

CRÉER/CLONER DES DÉPÔTS
=======================
Démarrer un nouveau dépôt ou en obtenir un depuis une URL existante

**$ git init [nom-du-projet]**
Crée un dépôt local à partir du nom spécifié

**$ git clone [url]**
Télécharge un projet et tout son historique de versions

EFFECTUER DES CHANGEMENTS
=========================
Consulter les modifications et effectuer une opération de commit

**$ git status**
Liste tous les nouveaux fichiers et les fichiers modifiés à commiter

**$ git add [fichier]**
Ajoute un instantané du fichier, en préparation pour le suivi de version

**$ git reset [fichier]**
Enleve le fichier de l'index, mais conserve son contenu

**$ git diff**
Montre les modifications de fichier qui ne sont pas encore indexées

**$ git commit -m "[message descriptif]"**
Enregistre des instantanés de fichiers de façon permanente dans l'historique des versions

**$ git commit -a -m "[message descriptif]"**
Enregistre des instantanés de tous les fichiers modifiés de façon permanente dans l'historique des versions

GROUPER DES CHANGEMENTS
=======================
Nommer une série de commits et combiner les résultats de travaux terminés

**$ git branch**
Liste toutes les branches locales dans le dépôt courant

**$ git branch [nom-de-branche]**
Crée une nouvelle branche

**$ git checkout [nom-de-branche]**
Bascule sur la branche spécifiée et met à jour le répertoire de travail

**$ git merge [nom-de-branche]**
Combine dans la branche courante l'historique de la branche spécifiée

**$ git branch -d [nom-de-branche]**
Supprime la branche spécifiée

VÉRIFIER L'HISTORIQUE DES VERSIONS
==================================
Suivre et inspecter l'évolution des fichiers du projet

**$ git log**
Montre l'historique des versions pour la branche courante

**$ git log --follow [fichier]**
Montre l'historique des versions, y compris les actions de renommage, pour le fichier spécifié

**$ git diff [premiere-branche]...[deuxieme-branche]**
Montre les différences de contenu entre deux branches

**$ git show [commit]**
Montre les modifications de métadonnées et de contenu inclues dans le commit spécifié

REFAIRE DES COMMITS
===================
Corriger des erreurs et gérer l'historique des corrections

**$ git reset [commit]**
Annule tous les commits après [commit], en conservant les modifications localement

**$ git reset --hard [commit]**
Supprime tout l'historique et les modifications effectuées après le commit spécifié

SYNCHRONISER LES CHANGEMENTS
============================
Référencer un dépôt distant et synchroniser l'historique de versions

**$ git fetch [nom-de-depot]**
Récupère tout l'historique du dépôt nommé

**$ git merge [nom-de-depot]/[branche]**
Fusionne la branche du dépôt dans la branche locale courante

**$ git push [alias] [branche]**
Envoie tous les commits de la branche locale vers GitHub

**$ git pull**
Récupère tout l'historique du dépôt nommé et incorpore les modifications
