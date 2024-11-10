Just a list of commands and my notes here

Configuring git
$ git config --global user.name "Your Name"
$ git config --global user.email "someone@email.com"
$ git config --list

Clone & Status
$ git clone <link>
$ git status

File Status
1. Untracked - New file(s) that git doesn't yet track
2. Modified - Changed
3. Staged - File is ready to be committed
4. Unmodified - Unchenged

Add & Commit
$ git add <--file_name-->     (adds new or changed files in your working directory to the got staging area)
$ git commit -m "message heading" -m "message description"       (it is the record of the change)

Push Command
$ git push origin main      upload the local repo content to remote repo

Initializing
$ git init
$ git remote add origin <--link-->
$ git remote -v          (to verify remote)
$ git branch             (to check branch)
$ git branch -M main     (to rename branch)
$ git push origin main

Quick Setup (Creating a new repository)
$ echo "#LocalRepo" >> README.md
$ git init
$ git add README.md
$ git commit -m "first commit"
$ git branch -M main
$ git remote add origin <--link-->
$ git push -u origin main

Quick Setup (Pushing an existing repository)
$ git remote add origin <--link-->
$ git branch -M main
$ git push -u origin main

Local Git Workflow
Git repo -> Clone -> Changes -> Add -> Commit -> Push

Branch Commands
$ git branch                             (to check branch)
$ git branch -M main                     (to rename branch)
$ git checkout <-branch_name->           (to navigate)
$ git checkout -b <-new_branch_name->    (to create a new branch)
$ git branch -d <-branch_name->          (to delete branch)

Merging Code
$ git diff <-branch_name->               (to compare commits, branches, files and more)
$ git merge <-branch_name->              (to merge two branches)

Pull Request -> it lets you tell others about changes you have pushed to branch in a repository on github

Pull Command
Used to fetch and download content from a remote repository and immediately update the local repo to match the content
$ git pull origin main

Resolving merge conflicts 
Done in an event that takes place when gt is unable to automatically resolve the differences in code between two commits
1. Pull Requests
2. Git Merge


Undoing Changes
Case 1: Staged Changes
$ git reset <-filename->
$ git reset

Case 2: Commited Changes (for one commit)
$ git reset HEAD~1

Case 3: Commited Changes (for many commits)
$ git reset <-commit_hash->
$ git reset --hard <-commit_hash->

Fork
- A fork is a new repositiry that shares code and visibility settings with the original "upstream" repository
- For is a rough copy
