# GitAndGithub
Basics of Git and GitHub.

### Version control system
- It is system that allows you to record changes to files over the time.
- Version control system(VCS) tracks the history of changes as people and team made.
- It tracks: which changes are made, who made the changes, when were the changes made, why were changes needed.

### Types of version control system
- There are three types of VCS: Local, Centralized and Distributed
- In Local Version control system, you manage all the version of files only within your local system. There is no remote server. All changes are recorded in local database. 
- In Centralized Version control system, you have a single "central" repository and each user get their own working copy. Whenever you commit the changes it will directly reflect to the central repository. To view the changes done to the repository, other users have to update it from central repository.
- In Distributed Version control system, there is a local copy of the repo for every developer on their own computer. They can make whatever changes they want and commit without affecting the remote repo. They first commit in their local repo and then push the changes to remote repo. 

### System failure of VCS
- In local VCS, if your hard disk gets corrupted or you lose the file, then you lose everything realted to it, including all the changes.
- In centralized VCS, if central repository goes down during development, collaboration will stop and if the hard disk of central repo becomes corrupted and you don't have any backup, you lose everthing and start from beginging.
- But in Distributed VCS, even if local repo is corrupted or remote repo does not work or is deleted, there is copy available with other developers. So you can take it from them, push to remote, and everything is back on track.
### Git, repository and Gihub
- Git is a free and open source distribute version control system.
- Repository is the collection of files and folder associated with a project, along with each file's revision history.
- Github allows us to host folders and files online. So, that all people/user around the world can contribute.

### Basic linux commands
- ls: list the folders present in repository.
- ls -a: it shows all hidden files.
- mkdir foldername: make the folder inside repo.
- cd foldername: change directory.
- touch filename.extension: to create file.
- vim filename.txt: to edit the text file.
- Esc + :w : this command is for vim editor. Helps in saving the file.
- Esc + :wq : this command is for vim editor. Helps in saving and quit the edited file.
- cat filename.txt: to check whats inside the file.
- rm -rf filename.extension: delete the file.

<b> All the operation which we perform like deleting, editing and making new files are stored in a folder which git provides (foldername: .git). So, how do we get this folder where all the history is stored? we have to intialize the folder by command: 'git.init' </b>

### Git commands
- git init: to intialize the folder so, that it can store history of file and folder
- git status: this command tell that these are all the changes which are currently not in the history of project and vice versa.
- Lets understand staging with help of example: At the wedding, there is a moment when some guest goes on the stage, the photographer clicks the guest photos with a couple, save them so that he can create the album and the guest leaves the stage after clicking the photo. 
So, similarly staging works in git. First we stage the file and then commit it for saving history. 
- git add . : it stage all the file present in repo.
- git add filename.extension: it stage specific file.
- git commit -m "any message realted to changes": it saves the history of file.
- git restore --staged filename.extension: it unstage the stage file,means it remove file from staged area.
- git log: to check all history of files.
- git reset hashcode_of_commit : it helps to remove the commit from history of log. But you can't specificly remove the middle commit. This command remove all the commit before the selected hashcode commit.Because each commit hash code is bulid up on each other.
- git stash: this command is useful when you don't want to lose new feature which are in staging area but also don't want to commit it right now. So, it will go to back stage area
- git stash pop: when you want feature back from backstage(stash).
- git stash clean: when you don't need your backstage code and delete it.<br>
### Commands for connecting local git repo to github repository. 
-  Create the new repository on github and copy its link. 
- git remote add origin copied link: here remote helps to connect the local git to remotly hosted repo, add refers adding new URL, origin refers to name of URL which we are copied from github(just like phone number, you don't remember all the numbers and keep a uniquie name for every constact).
- git remote -v: shows all URL associated with your repository.
- git push origin master/main: it make all changes visibile in github repository.

### Branches