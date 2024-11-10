Just a list of commands and my notes here <br />
<br />
<br />
Configuring git <br />
$ git config --global user.name "Your Name" <br />
$ git config --global user.email "someone@email.com" <br />
$ git config --list <br />

<br />
<br />

Clone & Status <br />
$ git clone <link> <br />
$ git status  <br />

<br />
<br />

File Status <br />
1. Untracked - New file(s) that git doesn't yet track <br />
2. Modified - Changed <br />
3. Staged - File is ready to be committed <br />
4. Unmodified - Unchenged <br />

<br />
<br />

Add & Commit <br />
$ git add <--file_name-->     (adds new or changed files in your working directory to the got staging area) <br />
$ git commit -m "message heading" -m "message description"       (it is the record of the change) <br />

<br />
<br />

Push Command <br />
$ git push origin main      upload the local repo content to remote repo <br />

<br />
<br />

Initializing <br />
$ git init <br />
$ git remote add origin <--link--> <br />
$ git remote -v          (to verify remote) <br />
$ git branch             (to check branch) <br />
$ git branch -M main     (to rename branch) <br />
$ git push origin main <br />

<br />
<br />

Quick Setup (Creating a new repository) <br />
$ echo "#LocalRepo" >> README.md <br />
$ git init <br />
$ git add README.md <br />
$ git commit -m "first commit" <br />
$ git branch -M main <br />
$ git remote add origin <--link--> <br />
$ git push -u origin main <br />

<br />
<br />

Quick Setup (Pushing an existing repository) <br />
$ git remote add origin <--link--> <br />
$ git branch -M main <br />
$ git push -u origin main <br />

<br />
<br />

Local Git Workflow <br />
Git repo -> Clone -> Changes -> Add -> Commit -> Push <br />

<br />
<br />

Branch Commands <br />
$ git branch                             (to check branch) <br />
$ git branch -M main                     (to rename branch) <br />
$ git checkout <-branch_name->           (to navigate) <br />
$ git checkout -b <-new_branch_name->    (to create a new branch) <br />
$ git branch -d <-branch_name->          (to delete branch) <br />

<br />
<br />

Merging Code <br />
$ git diff <-branch_name->               (to compare commits, branches, files and more) <br />
$ git merge <-branch_name->              (to merge two branches) <br />

<br />
<br />

Pull Request -> it lets you tell others about changes you have pushed to branch in a repository on github <br />

<br />
<br />

Pull Command <br />
Used to fetch and download content from a remote repository and immediately update the local repo to match the content <br />
$ git pull origin main <br />

<br />
<br />

Resolving merge conflicts <br /> 
Done in an event that takes place when gt is unable to automatically resolve the differences in code between two commits <br />
1. Pull Requests <br />
2. Git Merge <br />

<br />
<br />

Undoing Changes <br />
Case 1: Staged Changes <br />
$ git reset <-filename-> <br />
$ git reset <br />

<br />
Case 2: Commited Changes (for one commit)
$ git reset HEAD~1

Case 3: Commited Changes (for many commits)
$ git reset <-commit_hash->
$ git reset --hard <-commit_hash->

Fork
- A fork is a new repositiry that shares code and visibility settings with the original "upstream" repository
- For is a rough copy
