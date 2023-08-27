# In this repo will learn about GIT by answering a few questions.

1. How to remove a file from git after mentioning in Git.

* first mention it into gitignore file then run the following command

* Step 1:
    ```git
    git rm --cached remove_file.txt 
    ```
* Step 2:
    ```git
    git add .
    ```
* Step 3:
    ```git
    git commit -am "Remove ignored files"
    ```

* or in one line

```git
git rm -r --cached . && git add . && git commit -am "Remove ignored files"
```

2. How to remove a commit before push to git.
* There are three ways to do as mentioned below

1. Undo commit and keep all files staged:
```bash 
git reset --soft HEAD~
```
2. Undo commit and unstage all files:
```bash 
git reset HEAD~
```
3. Undo the commit and completely remove all changes:
```bash
git reset --hard HEAD~
```
