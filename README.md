# My Git Learning Repository 


##### create a new repository on the command line


	echo "# Test Repo" >> README.md

	git init

	git add README.md

	git commit -m "first commit"

	git branch -M main

	git remote add origin https://github.com/Sankarganesh2020/myrepo.git

	git push -u origin main


##### push an existing repository from the command line


	git remote add origin https://github.com/Sankarganesh2020/myrepo.git


	git branch -M main


	git push -u origin main






## Git commands


### GIT Cheat Sheet

 

##### init — Create an empty GIT repository in your development directory

Go to directory

	git init
 

##### status — Show the current state of the repository including un-added and un-committed files

	git status
 

##### add — Add a file to the repository staging area

Create a file, e.g. file.txt

	git add file.txt

Add all new or changed files to the repository staging area (the period means all)

	git add .
 

##### commit — Commit all changes to the repository for first time (-m means message)

	git commit –m “Initial commit”

##### Commit all changes to the repository for later activities

	git commit –m “Description of changes being made to project”
	
##### Push an existing repository

	git remote add origin https://github.com/Sankarganesh2020/myrepo
	git push -u origin master
 

##### branch — Create a new branch of the project

Choose a name for the new branch (original branch is master), e.g. test

	git branch test
	
List all branches (* appears next to current branch)

	git branch
 

##### checkout — Switch branches and check-out all files (e.g. to test branch)

	git checkout test

##### Create a new branch and check-out files in one command

	git checkout –b test
 

##### merge — Merge two branches together (go to the destination branch first, e.g. master)

	git checkout master
	
	git merge test
 

##### (delete) — Delete a branch that you no longer need (e.g. after a merge)

	git branch test –d

##### Or to force the delete:

	git branch test –D
 

##### log — View commit history (including long commit ID numbers)

	git log
 

##### revert — Revert all files back to a previous commit point

	git revert <long commit ID from the log command>


#####Removes cache from a specific file so that it can be added to the .gitignore

	rm -cache

##### Editing the configuration file

	git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author
	
##### git lg : A better way to display your git logs in your console. Command url : https://codingforeverybody.com/snippets/git-lg	
