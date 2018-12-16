## How do I get Git?
Git is one of the most popular version control systems in the software world, and that is the tool we will utilize in this organization.

*Note: This process is different if you have a mac or PC. Please follow the instructions accordingly.*
### Windows PC
Go to the link below, download git for windows, and click "Next" through the setup wizard.

https://gitforwindows.org/
### Mac OS
Go to your terminal. This can be accomplished by hitting <kbd>command</kbd> + <kbd>space</kbd> and by typing `terminal`. Git should already be installed on Mac OS, and you can check your version by typing

```shell
$ git --version
```
### Ubuntu or other Debian-based systems
Open your terminal and type:

```shell
$ sudo apt-get install git
```

## Verifying User Email

If you have never used GitHub before on your particular machine, you'll have to set the user email in your shell. Open your preferred shell (Git BASH, Terminal, etc.) and type:
```
$ git config --global user.email "<your-email-here@email.com>"
```

To confirm the email, type:
```
$ git config --global user.email
```

Congrats! You've successfully installed Git. 
