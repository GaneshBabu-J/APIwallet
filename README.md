#This File will help the developers to work on GitHub with Git.

Initially we shall have a master branch which will be the Production Ready Branch.
We shall follow git workflow strategy and create a development branch, which will be checkout version of the master branch.

Some of the Git Commands that are usefull are:
1. git clone <github-url> , its best to use ssh while cloning the repository.
   We can clone using either https or ssh. While doing it with https: a username and password will be prompted for the initial session where 
   the username and password needs to be entered. If session expires this activity keeps on repeating.
   If we try with ssh then this issue is over ruled.
   For this we need to create a ssh-key.
2. Command to create a ssh-key is
   ssh-keygen
3. Before doing that lets configure our email and username so we will have the correct permission on the repository to commit changes.
   git config --global user.name "username"
   git config --global user.email "email id"
   here we can replace global with local or we can leave that place empty. Which would mean it is set to only one repository.
   global will be for all the projects/repository that we are working on, local will be for a particular project.
4. So to create a branch.
   git branch -b <branch-name>; this will create a new branch.
   git checkout <branch-name>; will move to the newly create branch.
   Another command which will be easy is
   git checkout -b <branch-name>; will create a new branch and checkout.
5. to add files
   git add <file-name>; will add particular files
   git add . ; will add all the files
6. to commit the changes
   git commit -m "an appropriate message is required" ; here an appropriate message is required which would help the lead to track the changes required.
7. to push the changes
   git push <remote-name> <branch-name>
   most of the time remote-name will be origin
## Very important is that if more than one developer are working on the same branch then always before trying to push the changes to the remote its required that
## we should fetch/pull the details from the remote repository. So we can avoid the conflicts that might happen later.
   Command to pull the changes from the remote is
   git pull <remote-name> <branch-name>; pull will bring the changes to the local as well as working directory.
   git fetch <remote-name> <branch-name> ; will bring the changes to the local
## to get the changes to the working director
   git merge <branch-name> ; this will bring the changes to working directoy.
8. We can use the gitflow for the repository which will follow a unique workflow strategy.

