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

<b> All the operation which we perform like deleting, editing and making new files are stored in a folder which git provides (foldername: .git). So, how do we get this folder where all the history is stored? we have to intialize the folder by command: 'git.init' </b>

### Git commands
