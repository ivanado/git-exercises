
## Exercise 8: Merge or rebase feature branch

> ***If you prefer do the excercse in Visual Studio Code***

For this exercise you only need the local repository

## Setup:

1. Create new `exercise-8a` working directory
2. In the working directory initialize a local `exercise-8a` git repository

``` sh
# setup
mkdir exercise-8a
cd exercise-8a
git init
``` 

## Task:

1. add initial commit to `main` branch
``` sh
# initial commit
touch Readme.md
git add .
git commit -m "initial commit"
```
2. create a new branch, name it `feature-branch`
``` sh
# create branch
git checkout -b feature-branch
```
3. create 1 commit in `feature-branch`
``` sh
# commit in feature-branch
touch new-file.txt
git add .
git commit -m "add new-file"
```
4. create 1 commit in `main` again
``` sh
# switch to main and add new commit
git checkout main
touch hotfix.txt
git add .
git commit -m "add hotfix"
```
5. merge the commit from main into your `feature-branch`
``` sh
# switch back to feature-branch and get the latest commit from main
git checkout feature-branch
git rebase main
```
6. inspect the git log

7. create folder `exercise-8b` and repeat the exercise but use `merge` strategy instead of `rebase` in last step. What is the difference?
``` sh
# merge command with provided message for merge commit
git merge main -m "Merge branch 'main' into feature-branch"
```
8. compare the git logs in `8a` and `8b`

