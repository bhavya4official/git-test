# Git commands

## Setting up Git:
_(Downloading and Installing Git)_
>go to https://git-scm.com/downloads to download the Git installer for your specific computing platform and follow the installation steps.

## Global Configuration for Git:

>Open a cmd window or terminal on your computer.
_(Check to make sure that Git is installed and available on the command line)_
`git --version`

_(To configure your user name to be used by Git)_
`git config --global user.name "Your_User_Name"`

_(To configure your email to be used by Git)_
`git config --global user.email <your email address>`

_(You can check your default Git global configuration)_
`git config --list`
***

## Git operations on your Git repository:

>On your computer create a folder. Open this folder in any text editor and Create any file with some content.
_(Initializing the folder as a Git repository)_
`git init`

_(Checking your Git repository status)_
`git status`

_(To add files to the staging area of your Git repository)_
`git add .`
`git add --all`
`git add <file_name>`

_(To commit the current staging area to your Git repository)_
`git commit -m "first commit"`

_(To check the log of the commits to your Git repository)_
`git log --oneline`
`git log`
***

## Switch branches or restore working tree files:
_(Checking out a file from an earlier commit)_
`git checkout <commit's number first 7 digit> file_name`
`git checkout <commit's number first 7 digit>`

_(Resetting the Git repository)_
`git reset HEAD file_name`
`git reset` >(Reset the staging area to the last commit without disturbing the working directory)

_(Commit to the latest version)_
`git checkout -- index.html`
***

## Online GitHub/BitBucket repository to mirror local repository:
_(Set the local Git repository to set its remote origin)_
`git remote add origin <repository URL>`

_(Pushing your commits to the online repository)_
`git push -u origin master`
`git push --all`
***

## Make clone of git repository to local repository:
_(Cloning an online repository)_
`git clone <repository URL>`
