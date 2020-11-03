---
layout: post
title: Github - Basic commands
---
The windows portable git will work in most cases.

Initiate the git in the current folder. Right click and open the git bash. If on cmd, git init should work.
#### git init
Cloning the entire remote repo to a local location with root folder name as the repo name.
#### git clone https://github.com/rapidsailor/ShellScripts
 
Now navigate to the the newly created folders. Use cd command as needed.
Make some code chnages
To verify the changes and status
#### git status 

Add any new files to the repo or add the changes to exisitng files.
#### git add 

Commit the changes. Commits all the changes to the remote repo. This may ask for ur github user and password.
#### git commit -m "comment for check-in" 
Any file changes to be done using the vi, 
( i for insert mode, put in some comments. All the lines starting with # will be ignored. put some new lines without # as starting char.)
esc for going to command mode. :wq for saving and exiting.

Push the changes to remote master branch.
#git push origin master (this will push the data to remote repo)  

Pull the latest from the remote location.
#### git pull (Run this in the project folder)

Branching out and creating new branches.

View all the current branches
#### git branch

Create new branch. Below command will checkout the original code to new branch called branch1.
#git checkout -b branch1 (-b is used to create a new branch. To switch to an existing branch, remove -b)
After any code changes , run the following.
#### git add 
#### git commit -m "comment for check-in" 
#### git push -u origin branch1.

Setting the git configs
#### git config --global user.name "your full name"
#### git config --global user.email "your email"
