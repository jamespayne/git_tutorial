# git_tutorial

This is a test remote repository for the tutorial created by Corey Schafer which can be found [here](https://www.youtube.com/watch?v=HVsySz-h9r4&t=175s).

This was a refresher/practice for me to make sure my git skills are up to date

# Overview of Commands Learnt

## git

`git --version` Returns the version of git you are using.

## git config

`git config --global user.name "James Payne"` Sets the git config user name.
`git config --global user.email "test@test.com"` Stets the git config email.
`git config --list` Returns a list of config settings

## git help

`git help config` Gets help on the config command.
`git config --help` Another way of doing the command above.

## git init

`git init` Initializes a new repository in the current working directory.

## .gitignore

Adding a .gitignore file allows you to tell git what files to ignore such as:

    .DS_Store
    .project
    *.pyc

## git add

`git add -A` Adds all files to the staging area.
`git add somefile.txt` Adds a single file to the staging area.

## git status

`git status` Shows the current status of the repository.

## git reset

`git reset` Removes all files from the staging area.

## git clone

`git clone git@github.com:jamespayne/git_tutorial.git` Clones into a folder with the original name. e.g. git_tutorial
`git clone git@github.com:jamespayne/git_tutorial.git newname` Clones into a folder with a new name. e.g. newname

## git branch

`git branch -a` Shows all the branches of the repository

## Pushing/Pulling Changes

### git push and git pull

`git push origin master` Pushes the master branch to the remote master
`git pull origin master` Pulls the remote master branch

## Common Workflow

    # Pull the remote repository
    git pull git@github.com:jamespayne/git_tutorial.git

    # Create a new branch
    git branch new-feature

    # Check out the new-feature branch
    git checkout new-feature

    # Create a new file and make changes
    touch new-feature.txt && echo "This is a new feature." > new-feature.txt

    # Add the new file to the staging area
    git add -A new-feature.txt

    # Commit the new file with a detailed commit message
    git commit -m "Added the new file new-feature.txt and put some text in it"

    # Push the new branch upstream
    git push -u origin new-feature

    # Checkout and pull the master branch to avoid any conflicts
    git checkout master && git pull origin master

    # Merge the new branch
    git merge new-feature

    # Push the changes to remote master
    git push origin master
















