## Exercise 4: Resolving conflicts

> ***If you prefer do the excercse in Visual Studio Code***

If you have not yet create a repository and clone it on our machine following the steps from [0](../exercises/create_new_github_repo.exercise.md).

In this exerise git cannot figure out how to merge the content added on `conflict-branch` with the content on `main`.
Both changes need to be in `main` when you're done.


## Setup:

1. Make sure that you are using the `main` branch & run the following commands (or use VS Code): 
    - `git checkout main`
    - `touch greeting.txt`
    - `git add greeting.txt`
    - `git commit -m "Add file greeting.txt"`
    - `echo "hello" > greeting.txt`
    - `git add greeting.txt`
    - `git commit -m "Add content to greeting.txt"`
    - push the changes to your remote repo `git push origin main`
2. Run the folowing commands to create the `conflict-branch` with a new commit
    - `git checkout -b conflict-branch`
    - `echo "This is a relevant fact" > file.txt`
    - `git add file.txt`
    - `git commit -m "add relevant fact"`
    - push the changes to your remote repo `git push origin conflict-branch`
3. On the `main` branch run the following commands
    - `git checkout main`
    - `echo "This is an indispensable truth!" > file.txt`
    - `git add file.txt`
    - `git commit -m "add indispensable truth!"`
    - push the changes to your remote repo `git push origin main`


## Task:

1. Use `git merge` to bring the changes from `conflict-branch` on to `master`.
2. What does `git status` now report.
3. Fix the conflict with your favorite editor.
4. Follow the instructions in `git status` to complete the merge.
5. What does `git log --oneline --graph` show?
6. push the changes to your remote repo `git push origin main`
