# Basics of Git and Version Control
This document will give you the basics on Git, and how to push to and pull from the Github repository for Purdue Orbital.
## Why use Version Control?
Imagine this: typing `git pull` to pull the newest version of code, or going to the drive folder and wondering if the newest version is `test_code_fixed_NEW_FINAL.cpp` or `test_code_NEW_FINAL_REALFINAL(1).cpp`. Enough said.
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


## Adding Code to an Orbital Repository 
Let’s say you are going to create a new project to add to git. This is relatively straight forward. Navigate to the desired location, and use your shell (Git BASH for Windows, Terminal for Mac) to complete the following: 

1) To initialize an empty git repository in the current directory:

```shell
$ git init
```

2) To add all files within that directory to the git repository:

```shell
$ git add .
```

3) To commit your current changes:
```shell
$ git commit -m "Your custom commit message here"
```

4) To add a remote to point to your GitHub repo:
```shell
$ git remote add orbital https://github.com/purdue-orbital/my-new-repo-on-github.git
```

5) To push your changes to you GitHub remote:
```shell
$ git push orbital master
```

## Committing and Pushing New Changes on an Existing Remote
If you have already set a remote, then the process is even more simple:
```shell
$ git add .
$ git commit -m "Your custom commit message here"
$ git push orbital master
```

__More information on all of this can be found in our [wiki](https://github.com/purdue-orbital/Git-for-Orbital/wiki).__
