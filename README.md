# Git Learning Topics

## **Creating a Branch (Local)**

-   How to create a new branch locally:

    ``` bash
    git branch <branch-name>
    ```

-   How to switch to that branch:

    ``` bash
    git checkout <branch-name>
    # or
    git switch <branch-name>
    ```

------------------------------------------------------------------------

## **Creating a Branch on GitHub**

-   Pushing local branch to GitHub:

    ``` bash
    git push -u origin <branch-name>
    ```

-   Creating a branch directly on GitHub UI

------------------------------------------------------------------------

## **Working With Branches**

-   Adding and committing changes

    ``` bash
    git add .
    git commit -m "message"
    ```

-   Pushing multiple commits to a branch

    ``` bash
    git push
    ```

-   Checking branch differences

    ``` bash
    git diff
    git log
    ```

------------------------------------------------------------------------

## **Merging Branch to Main**

-   Merging your feature branch into `main`:

    ``` bash
    git checkout main
    git pull
    git merge <branch-name>
    ```

-   Fast-forward vs non-fast-forward merge\

-   Resolving merge conflicts

------------------------------------------------------------------------

## **Git Stash**

-   What is `git stash`\

-   Save uncommitted work:

    ``` bash
    git stash
    ```

-   View stashes:

    ``` bash
    git stash list
    ```

-   Apply stash:

    ``` bash
    git stash apply
    ```

-   Delete/Clear stashes:

    ``` bash
    git stash drop
    git stash clear
    ```

------------------------------------------------------------------------

## **Basic Git Commands**

-   Initializing a repository:

    ``` bash
    git init
    ```

-   Checking status:

    ``` bash
    git status
    ```

-   Adding files:

    ``` bash
    git add <file>
    git add .
    ```

-   Commit with message:

    ``` bash
    git commit -m "message"
    ```

-   Cloning repositories:

    ``` bash
    git clone <url>
    ```

-   Pulling latest changes:

    ``` bash
    git pull
    ```

-   Viewing history:

    ``` bash
    git log
    ```

------------------------------------------------------------------------

## **Remote Repositories**

-   Adding remote origin:

    ``` bash
    git remote add origin <url>
    ```

-   Fetch vs Pull\

-   Removing and renaming remotes:

    ``` bash
    git remote rename origin old-origin
    git remote remove origin
    ```

------------------------------------------------------------------------

## **Undoing Things**

-   Undo last commit:

    ``` bash
    git reset
    # or
    git revert <commit-id>
    ```

-   Remove file from staging:

    ``` bash
    git reset HEAD <file>
    ```

------------------------------------------------------------------------

## **.gitignore**

-   Why we use `.gitignore`\

-   Adding folders/files to ignore list\
    Example:

        /target
        /node_modules
        *.log
