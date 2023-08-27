# In this repo will learn about GIT by answering a few questions.

## 1. How to remove a file from git after mentioning in Git.

* The following commands will update the Git index while respecting Git ignores and remove every item from the Git index (but not from the working directory or local repository).

* Step 1:
    ```git
    git rm -r --cached .
    ```
* Step 2:
    ```git
    git add .
    ```
* Step 3:
    ```git
    git commit -am "Remove ignored files"
    ```
## 2. How to remove a commit before push to git.

* There are three ways to do as mentioned below

1. Undo commit and keep all files staged: 
```bash
git reset --soft HEAD~
```
* Undo commit and unstage all files: 
```bash
git reset HEAD~
```
* Undo the commit and completely remove all changes: 
```bash
git reset --hard HEAD~
```