# Travailler sur une branche en local

## Configuration
Installer cmder https://cmder.net/

Naviguer jusque dans un dossier de travail avec cmder 
```
cd [dir_sources]
```

Récupérer projet sur l’url (https://github.com/gregoryjacques/GitSample.git)
```
git clone https://github.com/gregoryjacques/GitSample.git
```

## Manipulation de branches
Basculer sur la branche develop
```
git chekcout develop
```
créer une branche feature_xxx
```
git checkout –b feature_xxx
```
Basculer sur cette branche
```
git checkout feature_xxx
```
## Etat des fichiers
Ouvrir un editeur et créer un nouveau fichier sample_[trigramme].txt
```
code .
```
Observer le statut du fichier
```
git status
```
Tracker le nouveau fichier
```
git add .
```
Observer le statut du fichier
```
git status
```
basculer sur la branche master
```
git checkout master
```
Observer le statut du fichier
```
git status
```
  basculer sur la branche develop
```
git checkout develop
```
créer un commit de votre modification
```
git commit –m "init first version"
```
basculer sur master
```
git checkout master
```
Observer le statut 
```
git status
```
basculer sur develop
```
git checkout develop
```
Observer le statut
```
git status
```
## Gestion des logs
voir les logs
```
git log 
git log --oneline –graph
```
# Gerer les modifications
basculer sur la branche feature_xxx
```
git checkout feature_xxx
```
modifier le fichier sample_[trigramme].txt en y ajoutant du texte et enregister

annuler ces changements
```
git reset –mixed
```
re-modifier à nouveau et commiter vos changements
```
git commit -m"mon deuxieme commit"
```
annuler ce commit
```
git reset --hard
```
Observer l'annulation de votre commit
```
git status
```

Layus sur le Head avec de multiples commit

Merge / rebase
