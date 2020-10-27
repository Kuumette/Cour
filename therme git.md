# Process git
![Grand Theft Life](git.png "GTL") 

# Definition des termes Git

## Workspace
Le Workspace ou Working Tree ou Working Directory est l'espace de travail. C'est une extraction unique d'une version du projet à partir de laquelle vous pouvez travailler. Ce dossier est stocké sur votre machine. Les fichiers ici sont soit identiques à la dernière révision enregistrée dans le dépôt local soit à l'état « Modifié ».

## Index
L'index ou Staging Area correspond à la liste complète des fichiers présents physiquement dans votre espace de travail qui ont été déclarés comme faisant partie de la prochaine révision que vous allez enregistrer. Il est donc possible qu'un fichier présent dans l'espace de travail ne soit pas présent dans l'index si vous ne l'avez pas ajouté. Les fichiers indexés sont dans un état « Indexé ».

## Local Repository
Le Local Repository est le dépôt local. C'est le dossier .git stocké dans votre espace de travail. C'est une réplique totale, sur votre machine, du dépôt distant. C'est dans le dépôt local que vous aller stocker vos révisions du projet. Le couple « .git » et l'espace de travail constitue ce que l'on appel le clone du dépôt distant. Les fichiers ici sont dans un état « Validé ».

## Remote Repository
Le Remote Repository est le dépôt distant. C'est le dossier dans lequel est stocké le projet sur le serveur qui fait office de référant. Vous ne pouvez pas directement modifier ces fichiers. C'est la référence lorsque vous clonez un projet sur votre environnement afin d'en créer une réplique local et d'en initialiser la révision la plus récente en tant qu'état des fichiers de l'espace de travail.

## add
Utiliser add permet d'ajouter des fichiers présent dans votre espace de travail vers l'index en prévisions d'une action futur vers un dépôt. Chaque fichier passe donc de l'état « Modifié » à « Indexé ».

## reset
Utiliser reset permet de retirer des fichiers de l'index ou annuler un instantané dans le dépôt local tout en conservant (ou non) les modifications faites. Pour annuler les modifications faites tout en laissant les index et dépôt local en place il faut utiliser revert.

## commit
Utiliser commit permet d'acter l'intégralité des fichiers de votre index dans le dépôt local en tant que nouvel révision. Chaque fichier passe donc d'« Indexé » à « Validé ».

## commit -a
Utiliser commit -a pour ajouter automatiquement la totalité des nouveaux fichiers à l'index puis les acter dans le dépôt local.

## push
Utiliser push pour monter et aligner l'intégralité des fichiers du dépôt local sur le dépôt distant.

## fetch
Utiliser fetch pour descendre et aligner l'intégralité des fichiers du dépôt local depuis votre dépôt distant.

## merge ou rebase
Utiliser merge pour fusionner les modifications présentent entre les fichiers de votre dernière révision et ceux rapatrier du dépôt distant (pour plus d'information sur la différence entre merge et rebase voir ici).

## pull [-r]
Utiliser pull pour descendre et ré-aligner les modifications présentent entre l'espace de travail, le dépôt local et le dépôt distant. En cas de conflit, l'action fetch aura été effectuée et vous devrez résoudre les conflits et utiliser merge vous même.

## checkout
Utiliser checkout permet d'extraire un instantané (une révision) et d'aligner l'espace de travail avec cet instantané du dépôt local depuis : la branche courante, une autre branche ou l'index.

## status ou diff
Utiliser status ou diff permet de comparer vos fichiers de l'espace de travail avec ceux de l'index ou du dépôt local. Vous pouvez ainsi voir ce qui a changé dans un comparateur de version.

## stash
Utiliser stash pour remiser l'état de votre espace de travail et de votre index dans la remise afin de ne pas perdre votre travail lors d'une extraction. Cela vous permet de ne pas acter un travail à moitié fini.


```git
fait apartir de l'ordi local :
git init ---> avoir un dossier propre
git remote ---> ajouté un repertoir distant 
git origin ---> nom referent quon donne au serveur 
git branch ---> ajouter une branch
git add *---> archive de se que je suis entrain de faire (indexer tout se qui vas etre commit)
git status ---> voir si ces ok (vert), nok(rouge)
git commit -m "..." ---> envoie d'une version (archive serveur local)
push ---> envoyer sur serveur distant 
git push --set-upstream origin master---> Si le push ne fonctionne pas.
git log ---> information se les commande faite voir tout les commit effectuer en grand
-----------------------------------------------------------------------------
fait apartir de github :
fork/clone ---> Copier local (premiere fois)recup le dossier .git
git add *
git commit
git push
-----------------------------------------------------------------------------
git pull ---> recupere des fichier mise a jour
git merger ---> fusionner un fichier
git log ---> information se les commande faite voir tout les commit effectuer en grand
git log --online ---> information se les commande faite voir tout les commit effectuer en petit
git diff ---> difference entre deux version (local et add)
git diff staged ---> difference entre deux version (add et commit)
git checkout ---> changer de branche
git config --global user.name.email
git config --global core.editor "chemain d'acces"--->logiel VSC
~ ---> dossier sources (c://utilisateur/manon/...)
```
```git
Gestion de branche



                    .---------.---------.-------------.------.
                    |                                 |      |
.---------------.----------------------.----------.----------.------------->
init
master
production
Fonctionalité1 .------.----------.-----.


Cle RSA ---> chiffrer / important (cle public(dechiffrer) et cle privée(chiffrer)) se connecter de facon securiser

cd (changer de dossier)
C://Users/manon/Documents/GitHub

$ git clone https://github.com/Manon04/Manon04.git
faire un clone 
git@github.com:Manon04/Manon04.git


git head ---> entete qui se deplace a chaque commit et pour faire un retour en arriere deplacer le head ou on veux en arriere 

git revert head^ ---> bouger le head de 1 en arriere cree un nouveau commit

hash/sha1/md5 ---> signature numero d'identification

git branch ... ---> creation d'une branche se posisionne sur le head 
```