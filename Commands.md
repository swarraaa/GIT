# Git Basic Commands:

### 1. Configure Git:

```bash
#username
git config --global user.name "first_name last_name"

#email
git config --global user.email "example@provider.com"
```

<hr/><br/>

### 2. Initailize an empty git repository:

```bash
#Initialise git
git init
```

<hr/><br/>

### 3. Staging the file:

```bash
#Add single file
git add <file_name>

#Add all the files in the current directory and any sub-directories
git add .

#Add all the files in the entire repository
git add -A
```

<hr/><br/>

### 4. Commit the staged files:

```bash
#Create new commit for the staged files
git commit -m "commit message"

#Skipping the staging area
git commit -a -m "commit message"

#Connect to last commit
git commit --amend
```

<hr/><br/>

### 5. Check status:

```bash
#Show status
git status

#Show short status
git status -s
```

<hr/><br/>

### 6. Check commit history:

```bash
#List of commits
git log

#-p or -- patch shows the difference introduced in each commit. -2 for 2 log entries
git log -p -2
```

<hr/><br/>

### 7. Check unstaged changes:

```bash
#Compare unstaged changes to staged changes
git diff

#Compare staged changes to  last commit
git diff --staged
git diff --cached
```

<hr/><br/>

### 8. Removing files:

```bash
#Stop tracking of file
git rm <file_name>

#Remove file from the staging area
git rm --cached <fiel_name>
```

<hr/><br/>

### 9. Moving files:

```bash
git mv file_from file_to
```

<hr/><br/>

### 10. Unstaging a staged file:

```bash
git reset HEAD <file_name>
```

<hr/><br/>

### 11. Unmodifying a modified file:

```bash
#Single file
git checkout -- <file_name>

#All files
git checkout -f
```

<hr/><br/>

# Remote Repositories:

### 1. Adding a remote:

```bash
git remote add <short_name> <url>
```

<hr/><br/>

### 2. View remote links:

```bash
#show the remotes
git remote

#Show the remotes with the links
git remote -v
```

<hr/><br/>

### 3. Cloning a repository:

```bash
#Make a copy of a remote repository and initialize git
git clone <remote_path>
```

<hr/><br/>

### 4. Getting contents of remote repository to local repository:

```bash
#Fetch the content from remote repository to local repository
git fetch <remote_name>

#Fetch and merge the content in local repository
git pull <remote_name>
```

<hr/><br/>

### 5. Pushing to your remotes:

```bash
#Push the changes in local repository to remote repository
git push <remote_name> <branch_name>
```

<hr/><br/>

### 6. Renaming and Removing remotes:

```bash
#Rename a remote
git remote <old_name> <new_name>

#Remove a remote
git remote remove <remote_name>
```

<hr/><br/>
