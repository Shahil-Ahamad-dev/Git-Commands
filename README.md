---

# **Git Commands Cheat Sheet**

---

## **Table of Contents**
1. [Setup and Configuration](#setup-and-configuration)  
2. [Repository Initialization](#repository-initialization)  
3. [Status and Changes](#status-and-changes)  
4. [Commits](#commits)  
5. [Logs and History](#logs-and-history)  
6. [Branching](#branching)  
7. [Merging](#merging)  
8. [Remote Repositories](#remote-repositories)  
9. [Viewing Differences](#viewing-differences)  
10. [Undoing Changes](#undoing-changes)  
11. [Stashing](#stashing)  
12. [Tags](#tags)  
13. [Advanced Commands](#advanced-commands)  
14. [Collaboration Commands](#collaboration-commands)  
15. [Additional Useful Commands](#additional-useful-commands)

---

## **1. Setup and Configuration**

### Set Your Name and Email
```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

### View or Edit Configuration
```bash
git config --list
git config --global --edit
```

---

## **2. Repository Initialization**

### Initialize a New Repository
```bash
git init
```

### Clone an Existing Repository
```bash
git clone <repository_url>
git clone --depth 1 <repository_url>  # Clone with minimal history
```

---

## **3. Status and Changes**

### Check Repository Status
```bash
git status
```

### Stage Changes
```bash
git add <file>    # Stage a specific file
git add .         # Stage all changes
git add -p        # Stage changes interactively
```

### Unstage or Discard Changes
```bash
git restore <file>           # Discard changes in the working directory
git restore --staged <file>  # Unstage a file
```

---

## **4. Commits**

### Commit Changes
```bash
git commit -m "Commit message"
```

### Commit All Changes
```bash
git commit -am "Commit message"  # Adds and commits all tracked files
```

### Amend the Last Commit
```bash
git commit --amend
```

---

## **5. Logs and History**

### View Commit History
```bash
git log
git log --oneline --graph --all  # Detailed log with branches
```

### View Changes in a Commit
```bash
git show <commit>
```

---

## **6. Branching**

### Manage Branches
```bash
git branch                        # List branches
git branch <branch_name>          # Create a branch
git checkout <branch_name>        # Switch to a branch
git checkout -b <branch_name>     # Create and switch to a branch
```

### Rename a Branch
```bash
git branch -m <new_branch_name>
```

---

## **7. Merging**

### Merge a Branch
```bash
git merge <branch_name>
```

### Resolve Merge Conflicts
When conflicts arise, resolve them manually in files and use:
```bash
git add <file>     # After resolving conflicts
git merge --continue
```

---

## **8. Remote Repositories**

### Synchronize Changes
```bash
git pull                         # Fetch and merge from the remote
git fetch                        # Fetch changes only
git push                         # Push local changes to remote
git push origin --delete <branch_name>  # Delete a remote branch
```

---

## **9. Viewing Differences**

### View Differences
```bash
git diff                         # Working directory vs staging area
git diff --staged                # Staging area vs last commit
git diff HEAD                    # All changes vs the last commit
```

---

## **10. Undoing Changes**

### Reset Commits
```bash
git reset <commit>               # Reset staging area to a specific commit
git reset --hard <commit>        # Reset staging area and working directory
```

### Undo the Last Commit
```bash
git reset --soft HEAD~1          # Keep changes in the staging area
git reset --mixed HEAD~1         # Keep changes in the working directory
```

---

## **11. Stashing**

### Save and Manage Stashes
```bash
git stash                        # Save changes temporarily
git stash list                   # List all stashes
git stash apply                  # Reapply the most recent stash
git stash pop                    # Apply and delete the most recent stash
git stash drop                   # Delete a specific stash
```

---

## **12. Tags**

### Manage Tags
```bash
git tag                          # List all tags
git tag <tag_name>               # Create a lightweight tag
git tag -a <tag_name> -m "Message"  # Create an annotated tag
```

---

## **13. Advanced Commands**

### Rebase Commits
```bash
git rebase <branch>              # Reapply commits on top of another branch
```

### Clean Untracked Files
```bash
git clean -f                     # Remove untracked files
git clean -fd                    # Remove untracked files and directories
```

---

## **14. Collaboration Commands**

### Debugging and Collaboration
```bash
git blame <file>                 # Show who last modified each line
git cherry-pick <commit>         # Apply a specific commit to the current branch
git shortlog -sn                 # Show contributor stats
```

---

## **15. Additional Useful Commands**

### Squash Commits
Combine multiple commits into one:
```bash
git rebase -i HEAD~<number_of_commits>
```

### Check File History
```bash
git log -- <file>                # See history of changes for a file
```

### Archive a Repository
```bash
git archive --format=zip HEAD -o repo.zip  # Create a zip archive of the repo
```

---

This enhanced version includes more commands for handling advanced workflows and common scenarios. Let me know if there's a specific use case you'd like addressed!
