# Rendu : lazarvb

- Dépôt : https://github.com/lazarvb/tp-git-1
- Site GitHub Pages : https://lazarvb.github.io/tp-git-1/

## Ex2

git log --oneline :

4b32293 (HEAD -> master) ex2: corrige une faute

21dd40a ex2: ajoute trois lignes

697d92e ex2: crée les notes

39bf8e7 ex1: initialise le dépôt

## Ex3

- config.local est-il encore dans l'historique ? Pourquoi ?

config.local est encore dans l'historique car même si on a arrêté de suivre ce fichier avec le .gitignore, cela n'enlève pas les anciens commits et pushs.

## Ex4

- git status après avoir retiré brouillon.txt du staging :

On branch master
Changes not staged for commit:
(use "git add <file>..." to update what will be committed)
(use "git restore <file>..." to discard changes in working directory)
modified: RENDU.md
modified: brouillon.txt

no changes added to commit (use "git add" and/or "git commit -a")

- Différence entre annuler une modification et retirer du staging ?

Annuler une modification veut dire que qu'on revient à comment était le fichier avant la modification, tandis que retirer du staging veut dire qu'on ne suit plus le fichier pour les commits et les pushs.

## Ex6

- À quoi servent <<<<<<<, ======= et >>>>>>> ?

Ces lignes sont ajoutées automatiquement pour montrer le conflit et les deux version concurrentes.

## Ex7

- git stash list (avant récupération) :

stash@{0}: WIP on master: 14848cb Revert "ex7: ajoute une ligne par erreur"

- Pourquoi annuler un commit plutôt que l'effacer de l'historique ?

Le but de Git est de garder une trace de tout, donc mieux vaut toucher à l'historique le moins possible.

## Ex8

- git pull = git fetch + git merge

## Ex10

git log --oneline --graph --all :

- 9ff986b (HEAD -> master) ex9: ajoute la page d'accueil
- ee2fd9e ex8: modification depuis GitHub
- 5e9449f Merge pull request #1 from lazarvb/feature-contact
  |\
  | \* a64fa93 (feature-contact) ex8: ajoute la page contact
  |/
- cbe5e6b ex7: ajoute la ligne en cours
  | _ f5ca992 (refs/stash) WIP on master: 14848cb Revert "ex7: ajoute une ligne par erreur"
  |/|
  | _ fc6d879 index on master: 14848cb Revert "ex7: ajoute une ligne par erreur"
  |/
- 14848cb Revert "ex7: ajoute une ligne par erreur"
- 21363ae ex7: ajoute une ligne par erreur
- a5b5407 ex6: résout le conflit du titre
  |\
  | \* 2e9995c ex6: titre en anglais
- | 7d8d06d ex6: titre en français
  |/
- a191be3 ex5: fusionne feature-menu
  |\
  | _ 501fd1d ex5: ajoute un dessert
  | _ 26265fc ex5: crée le menu
  |/
- e10bfb0 ex4: supprime a-supprimer.txt
- 3311e7c ex4: renomme ancien.txt
- 7bb3232 ex4: ajoute trois fichiers
- 091adbc ex3: arrête de suivre config.local
- 6c7c73c ex3: ajoute config.local (erreur)
- 2754e11 ex3: ajoute .gitignore
- 4b32293 ex2: corrige une faute
- 21dd40a ex2: ajoute trois lignes
- 697d92e ex2: crée les notes
- 39bf8e7 ex1: initialise le dépôt
