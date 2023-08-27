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

