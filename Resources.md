Git/GitHub Resources
=================

### Initial Setup

[https://help.github.com/articles/set-up-git](https://help.github.com/articles/set-up-git)

### Ignoring Files

If there are files in a repository that you don't want Git to track (e.g. temporary files, sensitive information, large files, etc.) you can create a _.gitignore_ file. 

While in your local repository create a file called _.gitignore_

```
nano .gitignore
```

In your _.gitignore_ file you can add file names or file types that should not be tracked by Git

```
filename.R
*.log
temp-*
```

If Git is already tracking a particular file, Git __will not__ ignore that file when it is added to your _.gitignore_ file. If you want Git to ignore an already tracked file, you must untrack the file with:

```
git rm --cached filename
```