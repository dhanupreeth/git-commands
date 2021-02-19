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
