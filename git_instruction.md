# GIT Instruction

    Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency. 

What is version control?

>Version control is a system that records
changes to a file or set of files over time so that you can recall specific versions later.

## Initializing GIT repository

In case you want to start controlling your project with Git, type

    git init

After this action a new folder named _**.git**_ that contains all of your necessary repository files will be created.

## Recording changes to the repository

To record changes to the repository it's necessary to add files and fix changes.

### Tracking new files

In order to begin tracking a new file, we use the command

    git add file_name

### Checking the status 

Checking the status is the main tool we use to determine which files are in which state. For checking the status we type command 

    git status

### Committing your changes

For commiting changes we type command

    git commit -m "text"

## Viewing the commit history

After you have created several commits you’ll probably want to look back to see what has happened. The most basic and powerful tool to do this is 

    git log

In case you want to see short history use the command

    git log --oneline

If you want to analyze merge history and graph of the branch type

    git log --graph
    
If it's necessary to see the difference between existing and changing files, type command

    git diff

## Git Branching

What is branching?
>Branching means you diverge from the main line of development and continue to do work without messing with that main line. 

### Basic branching

To create a new branch, type the command below:

    git branch branch_name

To check the existing branches use command:

    git branch

To switch to an existing branch we run command:

    git checkout branch_name

### Basic merging

After your work is complete and ready to be merged into master branch we can do the following steps:

* in case you want to merge into master branch, switch to master branch using command **git checkout master**
* check the branch typing **git branch**
* run **git merge branch_name** command

### Basic merge conflicts

What is merge conflict?

>If you change the same part of the same file in different branches, after merging you will face a merge conflict.

After merging information into master branch, for instance, you will see for options to solve this problem. These options are

* to accept current change
* to accept incoming change
* to accept both changes
* to compare changes

After choosing one of these options, commit changes using command **git commit -m "text"**

### Deleting branches

In case you have already merged the information from one branch into another and you don't need this branch anymore, you can use the command below:

    git branch -d branch_name

To check the number of existing branches you can always use command **git branch** 

## GitHub

What is GitHub?

    GitHub is the largest host for Git repositories, and is the central point of collaboration for millions of developers and projects. 

### Account setup

If you want to start working with GitHub, the first thing you need to do is to set up a free user account on website

[GitHub website](https://github.com/)

### Forking projects

In case you want to contribute to the project to which you don't have access, you can **fork** the project. It means that after forking the project you will get a copy of it. Now you are allowed to make changes to a project publicly.
To fork a project, visit the project page and click the “Fork” button at the top-right of the page.

### Git clone, Git Pull and Git Push functions

In case you want to work locally in Git after forking the project you need to do the following steps:

* open a necessary Folder in Git
* use **git clone url-address** command
* then type **cd name_folder** command

Now everything is ready to start working.

After you finish changing a file locally you need to use a command below to be able to see these changes on GitHub website as well

    git push 

Follow the system to see a full command

If you do changes on GitHub website use command below to see the changes in Git

    git pull

### Pull requests

After finishing all changes and saving them, visit GitHub, find a folder which was forked and press **contribute** button. Then choose green button **open pull request**. After comparing changes and possible discussions press **create pull request** to contribute.

## Conclusion

In case you need additional information about Git usage please follow the link and visit GIT website 

[Link to Git website](https://git-scm.com/)

Also you can download a free ProGit book which is available on out website.

