# Learning Git Notes
A set of notes I made while learning Git, and it is a reference for me when I want to review what I learned 😊

# Day 1
## / What is Git?
```
Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency.
```

## / Getting Help
```bash
# display all switches for config mode
user@system~$ git config -h
```

## / Configuring Git
```bash
# Set Username
user@system~$ git config --global user.name "0xGhazy"

# Set Email
user@system~$ git config --global user.email email@email.com

# Set the default editor
user@system~$ git config --global user.editor "code" # for vs code

# Read this answer https://stackoverflow.com/a/2825829/14071970
# Set the default Line ending
user@system~$ git config --global core.autocrlf True # for windows OS it's true, otherwise it's false
```

## / Git Workflow

### [+] Creating a new repository
inside the wanted directory execute the following command
```bash
# init a new repo in the CWD
user@system~$ git init
```

### [+] Staging files in staging area
adding Files to staging area to be able to commit them
```bash
user@system~$ git add <file-name> # for multiple files f1.txt f2.txt f3.txt
```

### [+] Commit your changes
```bash
user@system~$ git commit -m "message describes what you do"

# if you want to write a big message
user@system~$ git commit [ENTER] # will open the editor.
```
## / Notes
```
1/
When we commit our changes, files still in the staging area are not deleted
```

```
2/
Commit best practices
    - Don't do commits in each change. your commit must record a significant change such as 'adding a new feature' and 'fixing a bug'.

    - If we have a bug and typo error, in each one of these issues we do two separate commits for each issue
```

```bash
# If you want to commit your changes without adding your files to the staging area we use the following command

user@system~$ git commit -am
```
