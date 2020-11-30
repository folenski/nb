# GIT
##  Références
http://www.grafikart.fr   
http://rogerdudler.github.io/git-guide/index.html
##  Installation
### Linux pour ubuntu
`sudo apt install git-all`  
## Initialisation 
`git config --global user.email "Mario.Ferraz@hotmail.fr"`  
`git config --global user.name "Mario Ferraz"`  
`git config --global color.ui true`  
**Voir la configuration**  
`git config --global -l`  
## Utilisation  
**Voir le statut**  
`git status`  
**Ignorer les fichiers et/ou repertoires**  
`touch .gitignore`  
**doc ref** =>  https://linuxize.com/post/gitignore-ignoring-files-in-git/  
**Ajouter un element pour le commit**  
`git add README.md`  
**Ajouter n éléments pour le commit**  
`git add --all`  
**Faire le commit**  
`git commit -a  -m "1ere version conf conky"`  
## Visualisation du projet 
**Visualiser les modifications ( n pour l'histo)**  
`git log -n 2 --oneline`  
**Rechercher un élément**  
`git log -p README.md`  
## Revenir en arrière 
**Pour revenir en arrière en visualisation**, on prend l'ID : `git log --oneline` et `git checkout f823ef5 `  
**Défaire un commit** C'est uniquement les objets modifiés dans ce commit
`git revert f823ef5 `   !! Attention a ne pas confondre avec le **reset**, la il met le revert dans la pile, l'histo n'est pas oublié  
**Reset un commit**  les commits sont oubliés mais pas les modifications courantes  
`git reset f823ef5 `  
On peut uniquement faire un rollback sur un élément `git checkout f823ef5 config.php `  
Pour annuler la modif `git checkout master config.php ` 

Pour l'instant je travaille sur la branche master L'option -a sur le commit permet de prendre tous les fichiers modifiés Le git push envoie les fichiers vers le serveur

git push origin master


