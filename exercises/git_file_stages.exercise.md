## Exercise 2: Git file stages

In git, we are working with:

* The working directory where you are making your changes
* The staging area where all changes you have added through `git add` will stay
* The repository where every commit ends up, making your history. To put your staged changes in here you issue the `git commit` command.

A file can have changes both in the working directory and staging area at the same time.
These changes do not have to be the same.

We will also work with `git restore` to restore the staged changes of a file, and `git checkout` to return a file to a previous state.

## Setup:
1. Create a new `exercise-2` working directory
2. In the working directory initialize a local `excercise-2` git repository
3. In the working directory run the following
```bash 
echo 1 > file.txt
git add file.txt
git commit -m "1"
```


## Task:
1. What's the content of `file.txt`?
2. Overwrite the content in `file.txt`: `echo 2 > file.txt` to change the state of your file in the working directory (or `sc file.txt '2'` in PowerShell)
3. What does `git diff` tell you?
4. Run `git add file.txt` to stage your changes from the working directory.
5. What does `git diff` tell you?
6. Overwrite the content in `file.txt`: `echo 3 > file.txt` to change the state of your file in the working directory (or `sc file.txt '3'` in PowerShell).
7. What does `git diff` tell you?
8. Explain what is happening
9. Run `git status` and observe that `file.txt` are present twice in the output.
10. Run `git restore --staged file.txt` to unstage the change
11. What does `git status` tell you now?
12. Stage the change and make a commit
13. What does the log look like?
14. Overwrite the content in `file.txt`: `echo 4 > file.txt` (or `sc file.txt '4'` in PowerShell)
15. What is the content of `file.txt`?
16. What does `git status` tell us?
17. Run `git restore file.txt`
18. What is the content of `file.txt`?
19. What does `git status` tell us?
