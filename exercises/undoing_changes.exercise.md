# Exercise 3: Undoing changes

- `git commit --amend` enables changing of the last commit we made.
- `git reset` resets the last commit/s we made. More
  details [here](https://git-scm.com/book/en/v2/Git-Tools-Reset-Demystified).

You can use `git log -p` or `git show` to inspect the contents of commits and file changes that were added to the
commits.

## Setup:

1. Create a new `exercise-3` working directory
2. In the working directory initialize a local `excercise-3` git repository
3. In the working directory run the following
   - In PowerShell 
      - `Set-Content -Value "foo" -Path foo.txt`
      - `Set-Content -Value "bar" -Path bar.txt`
   - In others
     - `echo "foo" > foo.txt`
     - `echo "bar" > bar.txt`

## Task:

1. Run `git add foo.txt`
2. Run `git commit -m "feature 73"`
3. What does `git status` tell us?
4. What does `git log -p` tell us?
5. Stage the addition of bar.txt
6. Run `git commit --amend`
7. What happened? What does `git log -p` tell us?
8. What happens if you run `git commit --amend` again?
9. Run `echo "foofoo" > foofoo.txt` (or `Set-Content -Value "foofoo" -Path foofoo.txt` in PowerShell)
10. Run `git add foofoo.txt`
11. Run `git commit -m "feature 74"`
12. How does your working directory look like?
13. What does your log look like? What does your stage look like?
14. Try to run `git reset --soft HEAD~1`
15. What happens to your working directory, your log and your stage?
16. Run `git reset --hard HEAD~1`
17. What happens to your working directory, your log and your stage?
