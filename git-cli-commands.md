# Git Commands

## Git Syntax Highlighting
```bash
git config --global color.ui auto
```

## Remote
### Syncs branch to Remote
```bash
git fetch
```
### Lists all remotes
```bash
git remote
```
### Lists remote information (Example URL For Fetching & Push)
```bash
git remote -v
```
### Add remote
```bash
git remote add origin https://github.com/someuser/repo.git
```
### Removes Origin repo
```bash
git remote rm origin
```
### Shows where repository info is store
```bash
cat .git/config
```

### Cloning a new Repo
```bash
git clone https://github.com/someuser/repo.git
```
### Clone to a assigned directory
```bash
git clone https://github.com/someuser/repo.git assigneddirectory
```

### Branching
#### Lists Branches
```bash
git branch
```
### Create a New branch
```bash
git branch newbranch
```
### Switch to a branch
```bash
git checkout newbranch
```
### Creates and Switches to a new branch (named anotherbranch)
```bash
git checkout -b anotherbranch
```
### Discard local changes of a file
```bash
git branch -b newbranch origin/newbranch
```
### Creates new branch tracking a remote branch and switches to it
```bash
git checkout -b newbranch origin/newbranch
```

### Discard local changes of a file, replace by the version in another branch
```bash
git checkout somebranch -- filename.html
```
### Show all branches contained in the current branch
```bash
git branch --merged
```
### Renames branch
```bash
git branch -m oldname newname
```
### Shows remote branches
```bash
git branch -r
```
### Shows all branches (local and remote)
```bash
git branch -a
```
### Show path / reference to branch HEAD
```bash
cat .git/HEAD
```
### Lists directories / branches
```bash
ls -la .git/refs/heads
```
### Deleting
```bash
git branch -d branchtodelete
```
### Deletes branch regardless of unmerged content
```bash
git branch -D branchtodelete
```
## Comparing Commits
### Lists commits and SHA* in compact view
```bash
git log --oneline
```
### Lists commits and SHA* in compact view, showing all branches (‐‐all) in color
```bash
git log --graph --oneline --decorate --all
```
### Lists a certain number of remote’s commits in compact view
```bash
git log --oneline origin/master -3
```
### Show changes between a specific point in time to current working directory
```bash
git diff 871d36b
```
### Compares a file from a specific point in time to now
```bash
git diff 871d36b myfilename.php
```
### Compares a specific point in time to another point (range – from to)
```bash
git diff 871d36b..e7b1871
```
### Compares a file from specific point in time to another point (range – from to)
```bash
git diff 871d36b..e7b1871 myfilename.php
```
### Compares specific point in time to head
```bash
git diff 871d36b..HEAD
```
### Compares specific point in time to head, listing number of changes(‐‐stat) and files changed (‐‐summary)
```bash
git diff --stat --summary 871d36b..HEAD
```
### Compares specific point in time to head, ignoring whitespaces(-b) and all spaces(-w)
```bash
git diff -b -w 871d36b..HEAD
```
### Compares changes between branches
```bash
git diff master..anotherbranch
```
### Compares changes between branches showing inline color coded changes
```bash
git diff --color-words master..anotherbranch
```
### Compares changes between a branch and second to last commit in another branch
```bash
git diff master..somebranch^
```
### Compares remote and local branches
```bash
git diff origin/master..master
```
### Shows changes in a commit
```bash
git show 436eb47
```
### Shows only a certain number of commits (3 in this case)
```bash
git log --oneline -3
```


