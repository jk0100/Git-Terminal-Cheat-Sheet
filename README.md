# Git-Terminal-Cheat-Sheet

### Put remote branch on local machine:

`git clone <git@github.com:..>`
  
* Use ssh option, not url

### Checkout branch:

`git checkout <branch name>`

### See current branch:

`git branch`

* -a shows all branches

### Choose which files to commit

`git add path/to/your/file path/to/your/file ...`

`git add -A`

*Adds all files that were changed in directory

### Commit added files

`git commit -m 'your comment' path/to/your/file.txt`

* Commits a single added file

`git commit -m 'your comment'`

* Commits all added files

### Push commit to remote branch

`git push`

### Viewing commits:

`git status`

`git log`

### Updating local branch with master using rebase

`git checkout <local branch>`

`git rebase <master>`

`git push --force`

### Squashing commits:

`git rebase -i HEAD~<number of commits on branch>`

* select new (lower) commits to squash (replace 'pick' with 's')

* (optional) change commit message

`git push --force`

### Adding to single pushed commit

`git commit --amend`

* Make any changes to the message

`git push --force`

### Create new local branch and check it out

`git checkout -b new_branch_name`

### Fist commit on new branch created locally

`git push --set-upstream origin <new_branch_name>`

### Removing the last commit

`git reset --hard HEAD^`

* Can keep changes but undo the commit by removing the '--hard'

### Removing the last 2 commits

`git reset --hard HEAD~2`

### Merging branches

`git checkout <master>`

`git merge <branch>`

### Deleting a local branch

`git branch -d <branch>`
