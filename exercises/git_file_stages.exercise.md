## Exercise 2: Git file stages

In git, we are working with:

* The working directory where you are making your changes
* The staging area where all changes you have added through `git add` will stay
* The repository where every commit ends up, making your history. To put your staged changes in here you issue
  the `git commit` command.

A file can have changes both in the working directory and staging area at the same time.
These changes do not have to be the same.

We will also work with `git restore` to restore the staged changes of a file, and `git checkout` to return a file to a
previous state.

## Setup:

1. Create a new `exercise-2` working directory
2. In the working directory initialize a local `excercise-2` git repository
3. In the working directory run the following
   - In PowerShell
     - `Set-Content -Value "1" -Path file.txt`
   - In others
     - `echo 1 > file.txt`


## Task:

1. Run `git add file.txt`
2. Run `git commit -m "1"`
3. What's the content of `file.txt`?
4. Overwrite the content in `file.txt`: `echo 2 > file.txt` to change the state of your file in the working directory (
   or `sc file.txt '2'` in PowerShell)
5. What does `git diff` tell you?
6. Run `git add file.txt` to stage your changes from the working directory.
7. What does `git diff` tell you?
8. Overwrite the content in `file.txt`: `echo 3 > file.txt` to change the state of your file in the working directory (
   or `sc file.txt '3'` in PowerShell).
9. What does `git diff` tell you?
10. Explain what is happening
11. Run `git status` and observe that `file.txt` are present twice in the output.
12. Run `git restore --staged file.txt` to unstage the change
13. What does `git status` tell you now?
14. Stage the change and make a commit
15. What does the log look like?
16. Overwrite the content in `file.txt`: `echo 4 > file.txt` (or `sc file.txt '4'` in PowerShell)
17. What is the content of `file.txt`?
18. What does `git status` tell us?
19. Run `git restore file.txt`
20. What is the content of `file.txt`?
21. What does `git status` tell us?
