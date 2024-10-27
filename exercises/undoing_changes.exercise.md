# Exercise 3: Undoing changes

`git commit --amend` enables changing of the last commit we made.

You can use `git log -p` or `git show` to inspect the contents of commits and file changes that were added to the commits.


## Setup:
1. Create a new `exercise-3` working directory
2. In the working directory initialize a local `excercise-3` git repository
3. In the working directory run the following
```bash 
echo "foo" > foo.txt
echo "bar" > bar.txt
git add foo.txt
git commit -m "feature 73"
```
## Task:

1. What does `git status` tell us?
2. What does `git log -p` tell us?
3. Stage the addition of bar.txt
4. Run `git commit --amend`
5. What happened? What does `git log -p` tell us?
6. What happens if you run `git commit --amend` again?
