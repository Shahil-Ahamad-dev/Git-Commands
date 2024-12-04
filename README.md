# Git-Commands

---


## **Setup and Configuration**
- `git config --global user.name "Your Name"`  
  Set your name for Git.
- `git config --global user.email "your.email@example.com"`  
  Set your email for Git.
- `git config --list`  
  View your current Git configuration.

---

## **Repository Initialization**
- `git init`  
  Initialize a new Git repository.
- `git clone <repository_url>`  
  Clone a repository to your local machine.

---

## **Status and Changes**
- `git status`  
  Show the current status of the working directory and staging area.
- `git add <file>`  
  Stage a specific file.
- `git add .`  
  Stage all changes.
- `git restore <file>`  
  Discard changes in the working directory.
- `git restore --staged <file>`  
  Unstage a file.

---

## **Commits**
- `git commit -m "Message"`  
  Commit changes with a message.
- `git commit --amend`  
  Modify the last commit.

---

## **Logs and History**
- `git log`  
  View commit history.
- `git log --oneline`  
  View a simplified commit history.
- `git show <commit>`  
  Show details of a specific commit.

---

## **Branching**
- `git branch`  
  List all branches.
- `git branch <branch_name>`  
  Create a new branch.
- `git checkout <branch_name>`  
  Switch to a specific branch.
- `git checkout -b <branch_name>`  
  Create and switch to a new branch.
- `git branch -d <branch_name>`  
  Delete a branch.
- `git branch -D <branch_name>`  
  Force delete a branch.

---

## **Merging**
- `git merge <branch_name>`  
  Merge a branch into the current branch.

---

## **Remote Repositories**
- `git remote -v`  
  Show the list of remote repositories.
- `git remote add <name> <url>`  
  Add a remote repository.
- `git pull`  
  Fetch and merge changes from the remote repository.
- `git fetch`  
  Fetch changes without merging.
- `git push`  
  Push changes to the remote repository.
- `git push -u origin <branch_name>`  
  Push a new branch and set it to track the remote branch.

---

## **Viewing Differences**
- `git diff`  
  Show differences between the working directory and the staging area.
- `git diff --staged`  
  Show differences between the staging area and the last commit.

---

## **Undoing Changes**
- `git reset <commit>`  
  Reset the staging area to a specific commit.
- `git reset --hard <commit>`  
  Reset the staging area and working directory to a specific commit.
- `git revert <commit>`  
  Create a new commit that reverses a previous commit.

---

## **Stashing**
- `git stash`  
  Save changes in a temporary area and revert to a clean working directory.
- `git stash list`  
  View all stashed changes.
- `git stash apply`  
  Reapply the most recent stash.
- `git stash drop`  
  Delete the most recent stash.

---

## **Tags**
- `git tag`  
  List all tags.
- `git tag <tag_name>`  
  Create a lightweight tag.
- `git tag -a <tag_name> -m "Message"`  
  Create an annotated tag.
- `git push origin <tag_name>`  
  Push a tag to the remote repository.

---

## **Advanced Commands**
- `git rebase <branch>`  
  Reapply commits on top of another branch.
- `git reflog`  
  Show the history of HEAD references.
- `git bisect`  
  Perform a binary search to find a commit causing an issue.
- `git clean -f`  
  Remove untracked files from the working directory.

---

## **Collaboration Commands**
- `git blame <file>`  
  Show who last modified each line of a file.
- `git cherry-pick <commit>`  
  Apply a specific commit to the current branch.

---


