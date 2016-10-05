# README

This is a repo for learning and playing with git and GitHub.

---

* `git init` Initialize a git repository. Adds a `.git` folder to your working directory.
* `git status` Lists what tracked files have changes that are not staged
* `git add .`
* `git add -A`
* `git add -p`
* `git commit -m "Commit Message"`
* `git checkout -- .`
* `git log --graph --decorate --oneline --all`
* `git checkout -b newbranch`
* Merging
  * `git checkout (branch you want to merge changes INTO)`
  * `git merge (branch that contains committed changes of work you want)`
  * reminder: I like to merge master INTO the branch (checkout branch, merge master), make sure all is well, then merge branch into master (checkout master, merge branch).
* `git branch -d (branchname)`: deletes branch (safe)

---

### Working with GitHub

* `git remote -v` lists git remotes and associated urls
* `git remote add (name of remote) (ssh or https url)`
* `git push (name of remote) (name of branch)`
