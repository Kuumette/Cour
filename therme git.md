```git
fait apartir de l'ordi local :
git init ---> avoir un dossier propre
git remote ---> ajouté un repertoir distant 
git origin ---> nom referent quon donne au serveur 
git branch ---> pas sur la bonne branch
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