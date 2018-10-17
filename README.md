# Basics of Git and Version Control
This document will give you the basics on Git, and how to push to and pull from the Github repository for Purdue Orbital.
## What is Version Control?
Version control takes "snapshots" of the current state of your code in order to save changes, revert changes, and create working versions of software for current and future use. Another huge benefit is multiple people being able to simultaneously work on a piece of code at the same time.
## Why use Version Control?
Imagine this: typing `git pull` to pull the newest version of code, or going to the drive folder and wondering if the newest version is `test_code_fixed_NEW_FINAL.cpp` or `test_code_NEW_NEW_FINAL(1).cpp`. Enough said.
## Getting Started
Git is one of the most popular version control systems in the software world, and that is the tool we will utilize in this organization.
### Getting Git
*Note: This process is different if you have a mac or PC. Please follow the instructions accordingly.*
#### Windows PC
Go to the link below, download git for windows, and click "Next" through the setup wizard.

https://gitforwindows.org/
#### Mac OS
Go to your terminal. This can be accomplished by hitting <kbd>command</kbd> + <kbd>space</kbd> and by typing `terminal`. Git should already be installed on Mac OS, and you can check your version by typing

```shell
$ git --version
```
#### Ubuntu or other Debian-based system
Open your terminal, and type:

```shell
$ sudo apt-get install git
```

## Creating a GitHub Account
In order to pull shared files within our organizations, and to push changes to those same files, you must have a GitHub account. GitHub is simply an online resource that holds your git repositories on servers that can be accessed anywhere. Go to https://github.com to create a free account with your Purdue email. 

## Creating a repository
Lets say you are going to create a new project to add to git. This is relatively straight forward. Navigate to the desired location, and use your shell (Git BASH for Windows, Terminal for Mac) to complete the following: 



To initialize an empty git repository in the current directory:

```shell
$ git init
```

To add all files within that directory to the git repository:

```shell
$ git add .
```
Where `.` refers to all items within a directory. To add just one file, simply replace `.` with the name of the file you want to add (`git add my_file.c`)




