# Git commands

## Setting up Git:
_(Downloading and Installing Git)_

>go to https://git-scm.com/downloads to download the Git installer for your specific computing platform and follow the installation steps.

## Global Configuration for Git:
>Open a cmd window or terminal on your computer.

`git --version` _(Check to make sure that Git is installed and available on the command line)_

`git config --global user.name "Your_User_Name"` _(To configure your user name to be used by Git)_

`git config --global user.email <your email address>` _(To configure your email to be used by Git)_

`git config --list` _(To check your default Git global configuration)_

`git config credential.username username1` _(To switch git user)
***

## Git operations on your local Git repository:
>On your computer create a folder. Open this folder in any text editor and Create any file with some content.

`echo "# Project Description" >> README.md` _(To create a Readme file)_

`git init` _(Initializing the folder as a Git repository)_

`git status` _(Checking your Git repository status)_

`git add .`
`git add --all`
`git add <file_name/README.md>` _(To add files to the staging area of your Git repository)_

`git commit -m "Commit message"` _(To commit the current staging area to your Git repository)_

`git commit -a -m "Commit message"` _(Automatically stage files that have been modified and deleted - excluding new files)_

`git branch -M main` 

`git log --oneline`
`git log` _(To check the log of the commits to your Git repository)_
***

## Make a clone of git repository to the local repository:
`git clone <repository URL>` _(Cloning an online repository)_
***

## Online GitHub/BitBucket repository to mirror local repository:
`git remote add origin <repository URL>` _(Set the local Git repository to set its remote origin)_

`git pull <remote> <branch-name>` `git pull origin master` _(pulls the master branch from the remote called origin into your current branch)_

`git pull` _(git fetch+ git merge It fetch and download content from a remote repository and immediately update the local repository to match that content)_

`git push -u origin master` `git push --set-upstream origin master`
`git push --all`
`git push origin` _(Pushing your commits to the online repository)_

`git push -f origin master` _(Force change - override the remote branch code with your local repo code)_

`git remote -v` _(See the current configured remote repository for your fork)_
`git remote set-url origin <repo URL>`
`git remote remove origin` _(To remove remote)_
***

## Switch branches or restore working tree files:
`git branch` `git branch -r` _(To check all & working branch)_

`git branch <new-branch>` _(Create a new branch based on the current HEAD)_

`git checkout -b <new-branch-name>` _(To create and switch to a new branch)_

`git branch <new-branch> <base-branch>` _(create a new branch based on some existing one)_

`git checkout <branch-name>` _(To switch working branch)_

`git push origin <branch-name>` _(To push new branch to a remote repository)_

`git branch --set-upstream-to=origin/main <branch-name>` `git branch -u origin/main <branch-name>` _(<branch-name> will be set up to track 'origin/main' | set tracking information for this branch)_

`git checkout <commit's number first 7 digit> file_name`
`git checkout <commit's number first 7 digit>` _(Checking out a file from an earlier commit)_

`git reset HEAD file_name`
`git reset` _(Resetting the Git repository)_
 >It reset the staging area to the last commit without disturbing the working directory

`git checkout -- index.html` _(Commit to the latest version)_
***

## Error Fix: "main and master are entirely different commit histories"
```
git checkout master   
git branch main master -f    
git checkout main
git push origin main -f 
```
***
>Note: “origin” represents the default remote repository, typically the one you cloned from, while “upstream” refers to an additional remote repository that you may want to track or contribute changes to.
