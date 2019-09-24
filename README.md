# Working with Git

- [Basics](https://medium.com/@stevenpcurtis.sc/learning-the-essential-git-commands-d1adf4537e66)


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