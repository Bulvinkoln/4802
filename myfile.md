# GIT Operation Manual

## What is GIT?

**Git** is the most worldwide popular version control system (VCS) which enables using local repositories as well as remote ones.

**Repository Initialization**


 *git init*  command creates a new repository in the corresponding folder (a hidden folder .git).

**Committing modifications**

* *git add <file.name>* command enables modification monitoring by the system.

* *git status* command shows you the current state of the repository and the file status (untracked, modified, commited)

* *git commit -m "(message)"* command saves the last changes provided they were added with *git add* command. The message is **compulsory**!

* *git checkout <commit number>* command enables moving over versions.

* *git log* command demonstrates all the changes committed during the project creation.

## Git Branches

In order to work on the first draft and the final draft simultaniously or cooperate with colleagues, we can create several versions of the project. These versions are called branches.

### Branch creation
*git branch branch_name* command creates a new branch in the repository.

*git checkout -b branch_name* command creates and enters a new branch, which is more convenient and therefore used most often.

## Branch Merging

*git merge branch_name* command adds a new branch to the existing one.

## Branch Deleting
*git branch -d branch_name* command deletes the selected branch.

## Operating Remote Repositories at GitHub

### Creating a new account on github.com
Create your account on github.com following the instructions of the Sign Up section.

### Using a repository made by other people

Fing the repositury you want to use following the link or inserting its name into the search bar.

Press Fork button to copy the repository into your account.

### Sending the Remote Repository to Your Computer

Use *git clone (link)* command to create the identical local repository on you computer.

Use *cd (folder_name)* command to enter the exact folder in order to make changes in it.

### Working on the Local Repository

Create a new branch using *git checkout -b (branch_name)* command. You will make all changes in this branch only.

Create a new file in the folder with *touch (file_name)* command. The extension is optional.

Add the file to the git tracking with *git add .* command.

Add all necessary information into your file.

Commit the changes using *git commit -am "message"* command.

### Syncronizing the Remote Repository with the Local One

Send your version from the local repository to the remote repository with *git push --set-upstream origin branch_name* command. Another command to do the same: *git push -u origin branch_name*.

If you want to actualize the changes made from the local repository, use *git pull* command. From the remote repository, press _**Sync fork**_ button, then _**Update branch**_. 

In the remote repository press _**Pull Request**_ button in order to ask the owner of the project to accept your changes.