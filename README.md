# Git, GitHub and Version Control

## Version Control Overview
Version control in Git tracks changes to files and facilitates collaboration in software development. It allows reverting to previous versions when necessary, making it especially useful for teamwork.

--------
## Basic Git Workflow

### Create and Track a File
1. Create a folder and file:
```
cd Desktop
mkdir Story
cd Story
touch chapter1.txt
open -a /Applications/Visual\ Studio\ Code.app chapter1.txt

```

2. Initialise a Git repository and check the status:
```
git init
git status
```

3. Stage and commit changes:
```
git add .
git commit -m "Add the voucher"
```

### View Commit History
- To see the commit log:
```
git log
```

### Track Changes and Revert Modifications
1. Check for modifications:
```
git status
```
2. View Differences between versions:
```
git diff chapter1.txt
```

3. Revert changes to the last commimtted state:
```
git checkout chapter1.txt
```

---------------
## Remote Repositories 
### Linking a Remote Repository 
1. Add a remote repository:
```
git remote add <name> <url>
```

2. Push changes to the main branch:
```
git push -u origin main
```

---------------

## Ignoring Files
1. Create .gitignore file to exclude certain files:
```
touch .gitignore
```

3. Add the following entries to .gitignore:
```
.env
secrets.txt
```

3. Remove files from staging:
```
git rm --cached -r .
```

----------------

## Cloning a Repository

1. Clone a repository:
```
git clone <url>
cd <repo>
```

2. Install dependencies and set up:
Check the repository’s documentation for specific setup instructions.

-------------

## Branchign and Merging
### Creating and Switchign Branches

1. Create a new Branch:
```
git branch <name-of-branch>
```
   
2. Switch to the branch:
```
git checkout <name-of-branch>
```

### Merging Branches
1. Switching to the main branch:
```
git checkout main
```

2. Merge the branch into main:
```
git merge <name-of-branch>
```

### Log and save changes
1. View commit history:
```
git log
```

2. Quit and save:
```
:q!
```

## Push Changes
Push the updated branch to the remote repository:
```
git push origin main -u
```

## Forking and Pull Requests
Forking a repository allows you to create your own copy for experimentation or contribution. Once your changes are ready, you can submit a pull request to propose merging your updates into the original repository.








