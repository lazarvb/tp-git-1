# Rendu : lazarvb

- Dépôt : https://github.com/lazarvb/tp-git-1
- Site GitHub Pages :

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

## Ex7

- git stash list (avant récupération) :
- Pourquoi annuler un commit plutôt que l'effacer de l'historique ?

## Ex8

- git pull = git fetch + quoi ?

## Ex10

git log --oneline --graph --all :
