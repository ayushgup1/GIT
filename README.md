# GIT Commands
Basic GIT learnings

----------------------
## In your terminal play with these commands :

1. git --version  : It checks the version of the GIT running in your system. 
2. git clone url name  : To create a copy of repository in your local system. Replace url with HTTPS url and name with   the folder you want to keep in your local. 
3. git add README.md   : Moves file named README.md to staged area. 
4. git commit -m "message" : Moves file into commit zone with a particular message.
5. git push origin master : Pushes the staged files to master branch
 
## Now, after initial commit there are changes  : 

6. git diff README.md  : Shows diffrence in the files if any with respect to what you have in master branch.(working area and index/staged area) git diff --cached(index vs branch area)
7. git log   : Shows you the log history

If you want to move head to previous commit due to some issue with current commit use the following :

8. git checkout hashnumfromlog

## Fancy git log command modification : 
  
  git log --topo-order --all --graph --date=local --pretty=format:'%C(green)%h%C(reset) %><(55,trunc)%s%C(red)%d%C(reset) %C(blue)[%an]%C(reset) %C(yellow)%ad%C(reset)%n'

9. git reset HEAD NAME : to unstage the file. Replace NAME with the file you want to unstage. 
10. git checkout -- NAME : to recover the delected file.


## Branches

11. git checkout -b NAME : create a new branch with NAME
12. git checkout master  : moves to master branch
13. git branch           : highlights the branch you currently working in  
14. git push origin NAME

## Merging (Example from development branch to master branch)

15. git pull origin master  : Be upto date in mater branch
16. git merge development	: merge from development to master
17. git push origin master	: push the changes

## Remove the files

18. git rm --cached FILENAME : file removed from staged and back to working area. 

## Rename the files

    We had menu.txt already existing now we have changed its name to menu.md
19. git add menu.md
20. git add menu.txt  : adds empty menu.txt to staged area. Git automatically figures it out that it has been renamed. 

    OR 

21. git mv menu.txt menu.md : combination of 19 and 20
