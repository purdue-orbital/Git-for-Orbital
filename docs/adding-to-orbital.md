# How do I add my code to the page?

Once you have your code written on your local machine, you can then add it to the organization page to start tracking changes and versions. There are a few steps to add your code to the repo.

## Creating an Empty Git Repo

1) Open your shell. For Mac, use terminal (<kbd>command</kbd> + <kbd>space</kbd> and by typing `terminal`). For PC, open up Git BASH. If you need to install git, check out the [Installing Git](./getting-git.html) page. 

2) Navigate to the directory from the command line. For example, if the path for the directory is `Documents/Code/my-project`, the command to get to that directory would be:
```
$ cd Documents/Code/my-project
``` 

3) Initialize a new git repository by typing the following command into your shell:
```
$ git init
``` 
* All git commands will begin with the `git` keyword. `init` is just short for initialization. 
Make sure you are in the correct directory when you type this command.

## Committing to a Repository

Think of committing as creating a snapshot of how your code is at that current moment. For now, we want to commit everything that is in your particular directory so we can put it on the organization's page. Doing this is straight-forward.

1) In your root directory for your project (not in any sub-folders), run: 
```
$ git add .
``` 
* `.` refers to the current directory and all its contents. To just add one file specifically, just replace the `.` with the desired file name. For example, if we just wanted to add `my_file.c`, you would run `git add my_file.c`.
2) To see which files have been staged for committing, run 
```
$ git status
```
This allows us to see which files we are about to add, as well as confirm what files we are not adding. 
3) Once we have verified that what we have added is correct, run 
```
$ git commit -m "Initial commit"
```
* `Initial commit` is there just to show us that this is our very first commit into this repository. Later on, you can change this to whatever you'd like. Usually, it is a short description of what you have changed since the last commit. For example, if you fixed a rounding error in `my_file.c`, then your commit would look something like `git commit -m "Fix rounding error in my_file.c"`

Your file changes are now being tracked by git. This essentially means that every commit will act as a snapshot that can be accessed for different levels of debugging and redundancy.  

## Point Local Git Repository to GitHub Repository

To point your local repo to the one created on github.com/purdue-orbital, we need to reference the GitHub repository you created earlier on the website (refer [here](./github-for-orbital.html#empty-github-repository) if you don't remember).  For example, if you wanted to add the `Test-Repository` repo on Github, the command to do so would be:
```
$ git remote add origin https://github.com/purdue-orbital/Test-Repository.git
``` 
* `remote` simply refers to the fact that we are adding a web address to point our code to
*  `origin` is the name of the remote repository you are going to be pushing to. The naming convention is `origin`.

## Pushing Changes to GitHub
Finally, to get all those changes to the GitHub page, for a remote named `origin`, run:
```
$ git push origin master
```
Your code is now on the repository on our GitHub page! 
## Code Maintenance
Maintaining your code is also fairly simple, you would simply skip the "Creating an Empty Git Repo" and "Point Local Git Repository to GitHub Repository" steps. Whenever you make changes to your code in the repository, you will need to commit and push those changes to see them on the page. Refer to the [Committing to a Repository](./adding-to-orbital.html#committing-to-a-repository) and [Pushing Changes to GitHub](./adding-to-orbital#pushing-changes-to-github) steps.
