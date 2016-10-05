# README

This is a repo for learning and playing with git and GitHub.

pic here?

---

* `git init` - Initialize a git repository. Adds a `.git` folder to your working directory.
* `git status` - Lists the following items:
  1. tracked files with diffs that have been staged (added to the staging area)
  1. tracked files with diffs that are not staged
  1. untracked files (new files)
* `git add .` - Add all diffs in tracked and untracked files to staging area.
* `git add -A` - Same as above.
* `git add -p` - View diffs and add patch by patch to staging area.
* `git commit -m "Commit Message"` - Add all staged diffs to a commit with a message.
* `git checkout -- .` - Discard all changes in tracked files in the working directory.
* `git log --graph --decorate --oneline --all` - Best git command evah. The logs, with a graph of commits and branches, decorated with all pointers, each commit taking up oneline, including branches that are not checked out.
* `git checkout -b (newbranch)` - Create a new branch with specified name and check it out at the same time.
* `git checkout (branchname)` - Check out a branch that already exists.
* `git branch` - list all branches
* Merging
  * `git checkout (branch you want to merge changes INTO)`
  * `git merge (branch that contains committed changes of work you want)`
  * reminder: I like to merge master INTO the branch (checkout branch, merge master), make sure all is well, then merge branch into master (checkout master, merge branch).

---

### Working with GitHub

* `git remote -v` - List git remotes names and associated urls.
* `git remote add (name of remote) (ssh or https url)` - Add specified remote name and associated url. SSH is way cooler than https.
* `git push (name of remote) (name of branch)` - Push the work in specified branch to specified location.
* Getting remote work to your local machine (choose fetch and merge OR pull)
  * Fetch and merge
    * `git checkout (branch)`
    * `git fetch (name of remote) (name of branch - optional... leave off for all branches at that remote)`
    * `git merge (name of pointer... could be origin/master if you fetch origin master first)`
  * Pull (fetch and merge in one step)
    * `git checkout (branch))`
    * `git pull (name of remote) (name of remote branch)`
* `git push --delete (remote) (branchname)` - delete branch at specified remote repository
* `git branch -d (branchname)`: deletes branch (safe)
* `git branch -d -r (remote branch name)` - delete reference to remote branch
