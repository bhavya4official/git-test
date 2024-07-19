# Git commands

## Setting up Git:
_(Downloading and Installing Git)_

>go to https://git-scm.com/downloads to download the Git installer for your specific computing platform and follow the installation steps.

## Global Configuration for Git:
>Open a cmd window or terminal on your computer.

`git --version` _(Check to make sure that Git is installed and available on the command line)_

`git config --global user.name "Your_User_Name"` _(To configure your user name to be used by Git)_

`git config --global user.email <your email address>` _(To configure your email to be used by Git)_

`git config --list` _(You can check your default Git global configuration)_
***

## Git operations on your Git repository:
>On your computer create a folder. Open this folder in any text editor and Create any file with some content.

`echo "# ui-task-velocity" >> README.md` _(To create a Readme file)_
`git init` _(Initializing the folder as a Git repository)_

`git status` _(Checking your Git repository status)_

`git add .`
`git add --all`
`git add <file_name/README.md>` _(To add files to the staging area of your Git repository)_

`git commit -m "first commit"` _(To commit the current staging area to your Git repository)_

`git branch -M main` 

`git log --oneline`
`git log` _(To check the log of the commits to your Git repository)_
***

## Switch branches or restore working tree files:
`git branch` _(To check all & working branch)_

`git checkout -b <new-branch-name>` _(To create and switch to a new branch)_

`git checkout <branch-name>` _(To switch working branch)_

`git push origin <branch-name>` _(To push new branch to a remote repository)_

`git checkout <commit's number first 7 digit> file_name`
`git checkout <commit's number first 7 digit>` _(Checking out a file from an earlier commit)_

`git reset HEAD file_name`
`git reset` _(Resetting the Git repository)_
 >It reset the staging area to the last commit without disturbing the working directory

`git checkout -- index.html` _(Commit to the latest version)_
***

## Online GitHub/BitBucket repository to mirror local repository:
`git remote add origin <repository URL>` _(Set the local Git repository to set its remote origin)_

`git pull origin master` _(git fetch+ git merge It fetch and download content from a remote repository and immediately update the local repository to match that content)_

`git push -u origin master`
`git push --all`
`git push origin` _(Pushing your commits to the online repository)_
***

## Make a clone of git repository to the local repository:
`git clone <repository URL>` _(Cloning an online repository)_
