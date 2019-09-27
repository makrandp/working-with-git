# Working with Git

- [Basics](https://medium.com/@stevenpcurtis.sc/learning-the-essential-git-commands-d1adf4537e66)
- [Basics+](https://medium.com/datadriveninvestor/git-for-beginner-f438adfc3599)

## Alias
- [Git Aliases Reference 1](https://git-scm.com/book/en/v2/Git-Basics-Git-Aliases)
- [Git Aliases Reference 2](https://mijingo.com/blog/how-to-create-git-aliases)
- [Git Aliases Reference 3 - Medium Blog](https://koukia.ca/personalizing-git-aliasing-commands-4dda73b54081)
- My `~/.gitconfig`
```$xslt
[alias]
	st = status
	pu = config user.email "makrandapatil17@gmail.com"
	pu2 = config user.id "makrandp"
```

### Add file to staging 
- git add `filename`
### To unstage a file BEFORE COMMIT
- git rm --cached `filename` (this will remove file after the commit)
### To unstage a file AFTER COMMIT
- git reset HEAD -- `filename`

### Checkout remote branch
- git checkout --track origin/branch-name

### To discard changes to all files which are tracked and commited
- git checkout -- .
### To discard changes to a file which is tracked 
- git checkout -- `path/to/file`

## Scenario with Remove/Delete
### delete your tracked files
- git rm <file-path>
### If your file is in staging area then you have to give additional force flag.
- git rm <file-path> -f
###  delete files from git repository but not from your file system.
- git rm --cached <file-path>

## Git Logs
- git log --oneline
- git log --oneline --graph --decorate --all
### you want to see the commit message of a specific author
- git log --author="John Doe"

## Merge branch
### I always merge with --no-ff(no fast forward)
- git merge --no-ff <branch-name-to-merge> 

## Git reset
### Reset branch to a particular commit

