# git-basics


**If you consider a file in your Working Directory, it can be in three possible states.**

1. **It can be staged**. Which means the files with with the updated changes are marked to be committed to the local repository but not yet committed.

2. **It can be modified**. Which means the files with the updated changes are not yet stored in the local repository.

3. **It can be committed**. Which means that the changes you made to your file are safely stored in the local repository.

- **git add** is a command used to add a file that is in the working directory to the staging area.

- **git commit** is a command used to add all files that are staged to the local repository.

- **git push** is a command used to add all committed files in the local repository to the remote repository. So in the remote repository, all files and changes will be visible to anyone with access to the remote repository.

- **git fetch** is a command used to get files from the remote repository to the local repository but not into the working directory.

- **git merge** is a command used to get the files from the local repository into the working directory.

- **git pull** is command used to get files from the remote repository directly into the working directory. It is equivalent to a git fetch and a git merge .

## Step 0: Make a GitHub Account.

[github](https://github.com/)

## Step 1: Make sure you have Git installed on you machine.

$ git --version

**if not, try this command to install**

$ sudo apt install git-all

## Step 2: Tell Git who you are.

$ git config --global user.name "YOUR_USERNAME" 

$ git config --global user.email "username@gmail.com"

$ git config --global --list # To check the info you just provided

## Step 3: Generate/check your machine for existing SSH keys. (Optional)


## Step 4: Let’s Git

Create a new repository on GitHub. Follow this link.
Now, locate to the folder you want to place under git in your terminal

$ cd Desktop/giteg

**Initialize Git:**

$ touch README.md    # To create a README file for the repository

$ git init           # Initiates an empty git repository       

**Add files to the Staging Area for commit:**

$ git add .  # Adds all the files in the local repository and stages them for commit

OR if you want to add a specific file

$ git add README.md # To add a specific file

**Before we commit let’s see what files are staged:**

$ git status # Lists all new or modified files to be committed

**Commit Changes you made to your Git Repo:**

$ git commit -m "First commit"

**Uncommit Changes you just made to your Git Repo:**

$ git reset HEAD~1# Remove the most recent commit# Commit again!

## Add a remote origin and Push:

**Now each time you make changes in your files and save it, it won’t be automatically updated on GitHub. All the changes we made in the file are updated in the local repository. Now to update the changes to the master:**

**The git remote command lets you create, view, and delete connections to other repositories.**

$ git remote -v# List the remote connections you have to other repositories.

**The git remote -v command lists the URLs of the remote connections you have to other repositories.**

$ git push -u origin master # pushes changes to origin

**Now the git push command pushes the changes in your local repository up to the remote repository you specified as the origin.**

**See the Changes you made to your file:**

**Once you start making changes on your files and you save them, the file won’t match the last version that was committed to git. To see the changes you just made:**


$ git diff # To show the files changes not yet staged



