# GIT Commands
Basic GIT learnings

----------------------
In your terminal play with these commands :

1. git --version  : It checks the version of the GIT running in your system. 
2. git clone url name  : To create a copy of repository in your local system. Replace url with HTTPS url and name with   the folder you want to keep in your local. 
3. git add README.md   : Moves file named README.md to staged area. 
4. git commit -m "message" : Moves file into commit zone with a particular message.
5. git push origin master : Pushes the staged files to master branch
 
Now, after initial commit there are changes  : 

6. git diff README.md  : Shows diffrence in the files if any with respect to what you have in master branch. 
7. git log   : Shows you the log history

If you want to move head to previous commit due to some issue with current commit use the following :

8. git checkout hashnumfromlog