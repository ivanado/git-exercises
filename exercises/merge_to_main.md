
## Exercise 7: Merge to main

> ***If you prefer do the excercse in Visual Studio Code***

For this exercise you only need the local repository

## Setup:

1. Create new `exercise-7` working directory
2. In the working directory initialize a local `exercise-7` git repository

``` sh
# setup
mkdir exercise-7
cd exercise-7
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
2. create a new branch, name it `dev-branch`
``` sh
# create branch
git checkout -b dev-branch
```
3. create 1 commit in `dev-branch`
``` sh
# commit in dev-branch
touch new-file.txt
git add .
git commit -m "add new-file"
```
4. merge this commit into `main`
``` sh
# merge to main
git checkout main
git merge dev-branch
```
5. inspect the git log
6. delete the `exercise-7` folder and start the exercise again using vscode git UI to achieve the commits and merge 




