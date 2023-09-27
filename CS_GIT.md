# Git Cheat Sheet

## Git Configuration

Set your name
```bash
git config --global user.name "Your Name"
```
Set your email address
```bash
git config --global user.email "youremail@example.com"
```

## Creating and Cloning Repositories

Initialize a new Git repository in your current directory
```
git init
```
Clone an existing repository from a remote URL
```
git clone <remote_url>
```

## Basic Workflow

Check the status of your repository
```
git status
```
Add changes to the staging area
```
git add <file_name>
```
Commit changes with a message
```
git commit -m "Your commit message"
```
Push changes to a remote repository
```
git push <remote_name> <branch_name>
```
Pull changes from a remote repository
```
git pull <remote_name> <branch_name>
```

## Branches

Create a new branch
```
git branch <branch_name>
```
Switch to a different branch
```
git switch <branch_name>
```
Create and switch to a new branch
```
git checkout -b <branch_name>
```
List all branches (local and remote)
```
git branch -a
```
Delete a branch
```
git branch -d <branch_name>
```

## Merging and Rebasing

Merge a branch into the current branch
```
git merge <branch_name>
```
Rebase your current branch onto another branch
```
git rebase <branch_name>
```

## Remote Repositories

List all remote repositories
```
git remote -v
```
Add a new remote repository
the remote_name is often "origin"
```
git remote add <remote_name> <remote_url>
```
Remove a remote repository
```
git remote remove <remote_name>
```

## History and Log

View a log of commits
```
git log
```
Show the changes in a specific commit
```
git show <commit_hash>
```

## Discard Changes

Discard changes in the working directory for a specific file
```
git checkout -- <file_name>
```
Discard all changes in the working directory
```
git reset --hard HEAD
```
