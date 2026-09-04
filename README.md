# *** Git Notes ** 

A concise, step-by-step guide to essential Git commands and concepts based on practical handwritten notes.
---
## 1. Basic Git Workflow & Commands

| Step / Command | Usage | Description |
| :--- | :--- | :--- |
| *git init* | git init | Initialize a new local Git repository to track changes. |
| *git status* | git status | Check the current status of files (untracked, modified, staged). |
| *git add* | git add <filename> | Stage file changes for the next commit. |
| *git commit* | git commit -m "commit msg" | Commit staged changes to local repository history. |
| *git diff* | git diff | Show changes between working directory and staging area. |
| *git rm* | git rm --cached <filename> | Remove file from staging area without deleting local file. |
| *git remote* | git remote add origin <url> | Connect local repository to a remote repository URL. |
| *git push* | git push origin main | Upload local commits to remote branch (main or any branch). |
| *git clone* | git clone <ssh/https-url> | Copy a remote repository to your local machine. |

---
## 2. Remote Operations & Concepts
* *Pull vs. Fetch*
  * *git pull: Downloads latest code from remote **and* automatically merges it into your current working branch.
  * *git fetch: Downloads information and code from remote **without* merging into your branch.
* *Clone vs. Fork*
  * *Clone*: Creates a local copy of a remote repository on your personal machine.
  * *Fork*: Creates a server-side copy of another user's Git repository under your own remote account.
---
## 3. Git Branching
1. *Create Branch*: git branch <branch-name> (e.g., git branch feature-login)
2. *Switch Branch*: git switch <branch-name> or git checkout <branch-name>
3. *Create & Switch*: git checkout -b <branch-name> or git switch -c <branch-name>
4. *List Branches*:
   * Local: git branch
   * Remote: git branch -r
5. *Delete Branch*: git branch -d <branch-name>
6. *Push Branch to Remote*: git push origin <branch-name>
---
## 4. Merging Branches
1. Switch to target main branch: git checkout main
2. Fetch latest changes first: git pull origin main
3. Merge feature branch into main: git merge <branch-name>
4. Note: Resolve any merge conflicts manually if prompt appears.
---
## 5. Git Rebase vs. Merge
* *git rebase <branch-name>*: Rewrites commit history into a clean, linear single-line sequence over main branch without merge commits.
* *git merge <branch-name>*: Preserves full commit history, creating a distinct merge commit node.
---
## 6. Git Stash
Temporarily saves working directory modifications without committing so you can switch branches cleanly.
* *Save changes*: git stash
* *List stashes*: git stash list
* *Re-apply saved changes*: git stash apply
