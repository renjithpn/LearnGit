# Git Commands


#### Initial Configuration

git config --global user.name "Sam Smith"
git config --global user.email sam@example.com

#### Create a new local repository	 	
git init

#### Check out a repository	Create a working copy of a local repository	
git clone /path/to/repository
For a remote server, use:	
git clone username@host:/path/to/repository


#### Add files	Add one or more files to staging (index)	


### Branches
git checkout -b branchname : Create a new branch and switch to it.
git checkout branchname    : Switch from one branch to another.	 
git branch  : List all the branches in your repo, and also tell you what branch you're currently in.
	
git branch -d branchname   : Delete the feature branch.

git push origin branchname : Push the branch to your remote repository, so others can use it.
Push all branches to your remote repository:	
git push --all origin
Delete a branch on your remote repository:	
git push origin :branchname



### Update from the remote repository
Fetch and merge changes on the remote server to your working directory:	git pull
To merge a different branch into your active branch:	
git merge <branchname>
View all the merge conflicts:
View the conflicts against the base file:
Preview changes, before merging:
git diff
git diff --base <filename>
git diff <sourcebranch> <targetbranch>
After you have manually resolved any conflicts, you mark the changed file:	
git add <filename>
