# Basic Git commands
*This file contains every basic git commands for everyday use*

## Cloning a Repo
To clone a repo we use the `git clone` command
- this command can be use to clone our repo as well as other people's repo
### The syntax
> for personal repo
```
git clone https://{PAT}@github.com/{username}/{repository}.git
```
> for other people's repo
```
git clone https://github.com/{username}/{repository}.git
```

## Staging/Adding a file
to stage or add a file for git to track use `git add` This is used to make git track a file and follow all changes
### The syntax
> To add one file
```
git add filename
```
> to add multiple file
```
git add .
```

## Checking file Status
The git command `git status` is used to check the status of a file. whether it have been staged or not and commited or not. also checks the status of working tree
### The syntax
```
git status
```

## Commiting a file
The command for commiting a file is `git commit`. this is used to commit all staged file to git. a committed file can be tracked with it's automatically generated hash key for later use
### The syntax
> To just commit with a message
```
git commit -m "message
```
- the flag *-m* stands for message with the expected message within a quotataion marks
- the messages are identifies for what that commit is all about
> To add and commit an already tracked file
```
git commit -a -m "message" 
```
- the *-a* is for add

## Pushing to github or any remote repo
The command `git push` is used to push our commit to any remote repositories like github or gitbucket
### The syntax
> Repo with single branch and automatic upsteam
```
git push
```
> repo with multiple branch and non generic upstream name *i.e: origin* 
```
git push upstream-name branch-name
```