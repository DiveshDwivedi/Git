## Git Commands and It's Use 

### git init 

This command use, if you want to start a new empty repository or to reinitialize an existing one in the project root. It will create a .git directory with its subdirectories.

### git config --global user.name "Your_Name"

Define the author name to be used for all commits by the current user.

### git config --global user.email "Your_Email"

Define the author email to be used for all commits by the current user.

### git status

List of all changes in local which files are staged, unstaged, and untracked.

### git diff

Show unstaged changes between your index and working directory.
It helpfull to see whats new changes performed, by compairing to older.

### git add <directory>

Stage all changes in <directory> for the next commit. 
Replace <directory> with a <file> to change a specific file.
To stage specific <file> for commit.

### git add .

Add all changes in <directory> to stagged at once for the next commit.
All changes are stagged for commit. 

### git commit -m <"message">

Commit the staged snapshot, but instead of launching a text editor, use <message> as the commit message.

Replace <"message"> with "commit message".

Commit message should follow related task or change.

### git commit --amend -m "new_commit_message"

Change commit message in local.

Replace the last commit with the staged changes and last commit combined. Use with nothing staged to edit the 
last commit’s message

### git remote add <name> <url> Or git remote add origin <url_or_ssh>

Create a new connection to a remote repo. After adding a remote, 
you can use <name> as a shortcut for <url> in other commands.

Create a new Repo on remote and connect with local. 

### git branch

List all of the branches in your repository.

### git branch <new_branch_name>

Create a new branch with the given name(<new_branch_name>).
Branch name should relate to your work.

### git branch -m <old_branch_name> <new_branch_name>

Rename a branch while pointed to any branch.

### git checkout <branch_name>

Switch on branch named <branch_name>.

### git checkout -b <branch_name>

Create and check out a new branch named <branch_name>.

### git branch -d <branch_name>

First make sure you are not on that banch.
To delete branch named <branch_name>.

### git push origin --delete <remote_branch_name> or git push <remote_name> : <remote_branch_name>

Delete branch named <remote_branch_name> from remote.

### git push origin <branch_name> or git push --set-upstream orign <branch_name>

Push the branch to <remote>, along with necessary commits and objects. Creates named branch in the remote repo if it doesn’t exist.

### git pull 

This is a shorthand for pulling commits into local branch that is tracking a remote branch.

### git pull origin master

Let's say you are on local/master, and run this command, git will fetch commits from origin/master and then merge it into local/master.

### git stash

If some change don't want to commit but keep changes for future use(commit).

### git stash push <paths_you_wish_to_stash>

From multiple changes you don't want to commit some, then stash that by [paths you wish to stash e.g. src/] for future commit.

### git stash list

Lists all stashed file or directory.

### git stash clear

To clear all stashed lists.

### git reset

Reset staging area to match most recent commit, 
but leave the working directory unchanged.

### git reset --hard

Reset staging area and working directory to match most recent commit and overwrites all changes in the working directory.

To discard all recent change in working directory.


### git checkout master && git pull 

Switch on master branch and pull once. 
Change branch name as your need.

### git clone <repository_url>

Clone repo located at <repo> onto local machine. Original repo can be 
located on the local filesystem or on a remote machine via HTTP or SSH.

Clone remote repository into your local.

### git fetch

Get all the updates from the remote repository, including new branches.
