

---

# **Git Commands Cheat Sheet**

A comprehensive guide to common Git commands for setup, repository management, collaboration, and troubleshooting.

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

---

## **1. Setup and Configuration**

### Set Your Name and Email
```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

### View Configuration
```bash
git config --list
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

### Amend the Last Commit
```bash
git commit --amend
```

---

## **5. Logs and History**

### View Commit History
```bash
git log
```

### Simplified Commit History
```bash
git log --oneline
```

### Show Details of a Specific Commit
```bash
git show <commit>
```

---

## **6. Branching**

### List Branches
```bash
git branch
```

### Create a New Branch
```bash
git branch <branch_name>
```

### Switch Branches
```bash
git checkout <branch_name>       # Switch to an existing branch
git checkout -b <branch_name>    # Create and switch to a new branch
```

### Delete a Branch
```bash
git branch -d <branch_name>      # Safe delete
git branch -D <branch_name>      # Force delete
```

---

## **7. Merging**

### Merge a Branch
```bash
git merge <branch_name>
```

---

## **8. Remote Repositories**

### Manage Remotes
```bash
git remote -v                    # Show remote repositories
git remote add <name> <url>      # Add a new remote repository
```

### Synchronize Changes
```bash
git pull                         # Fetch and merge changes from the remote
git fetch                        # Fetch changes without merging
git push                         # Push changes to the remote
git push -u origin <branch_name> # Push a new branch and track it remotely
```

---

## **9. Viewing Differences**

### View File Differences
```bash
git diff                         # Working directory vs staging area
git diff --staged                # Staging area vs last commit
```

---

## **10. Undoing Changes**

### Reset or Revert Changes
```bash
git reset <commit>               # Reset staging area to a specific commit
git reset --hard <commit>        # Reset staging area and working directory
git revert <commit>              # Create a new commit to reverse a specific commit
```

---

## **11. Stashing**

### Manage Stashes
```bash
git stash                        # Save changes temporarily
git stash list                   # View all stashes
git stash apply                  # Reapply the most recent stash
git stash drop                   # Delete the most recent stash
```

---

## **12. Tags**

### Manage Tags
```bash
git tag                          # List all tags
git tag <tag_name>               # Create a lightweight tag
git tag -a <tag_name> -m "Message" # Create an annotated tag
git push origin <tag_name>       # Push a tag to the remote
```

---

## **13. Advanced Commands**

### Advanced Operations
```bash
git rebase <branch>              # Reapply commits on top of another branch
git reflog                       # Show history of HEAD references
git bisect                       # Binary search to find a problematic commit
git clean -f                     # Remove untracked files
```

---

## **14. Collaboration Commands**

### Collaboration and Debugging
```bash
git blame <file>                 # Show who last modified each line
git cherry-pick <commit>         # Apply a specific commit to the current branch
```

---

This enhanced version is optimized for readability and usability while keeping the information concise. Let me know if you'd like any additional modifications!
