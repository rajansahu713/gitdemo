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

## 3. How to remove commit after push the changes.
* You may see a message similar to the image below. This is called a COMMIT_EDITMSG; it holds a commit message of a commit in progress. It includes information about the commit that you’re reverting, including the author, the branch, the file, and the message. The goal for you is to review it and close the commit editor.

* If this file opens in your IDE, you can just close the file at the top. If you’re seeing this message in your terminal via Vim, you can use the command 

Step 1:
```bash
git revert 0a3dbc774ea29bfd68fe55caf1ade33dba1bda35
```

step 2:
```bash
git push
```

4. How to delete a branch.
* for renaming the branch you need to other branch than deleting one.
```bash
git branch -d checkout123
```


* To rename the branch always remember you that you must on that branch otherwise you are not able to delete.

```bash
git branch -m bug2023
```



5. what is fast forward 