<strong>#Pour identifier le commit qui a tout fait foirer </strong>
- git stash : stock v en cours
- git log : consulter numeros commits
- git checkout + numero commit :on revient sur les files de ce commit
- git checkout master
- run tests
- git stash pop : restaure version initiale
A faire : tester la difference git checkout et git checkout master

<strong>#force a push</strong> \
git push --force

<strong>#Branches</strong> \
git checkout -b BRANCH_NAME - creer une branche\
add, push... \
git push --set-upstream origin BRANCH_NAME

<strong>#Team work</strong> 
git checkout BRANCH_NAME - se deplacer dans une branche \
git checkout master - retour au master \
git pull - mettre a jour son master pour recup ce qui a ete merge par les autres \
git merge BRANCHE, puis git push - push sa branche \
git checkout BRANCH - retour branche \
git merge master - recuperer son push ainsi que les autres push sur le master, dans la branche

<strong>#Voir tous les commits sur un fichier</strong> 
git log -p monFichier
