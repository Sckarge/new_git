# Made in VSCODE

**How great is this...**

Git has the following commands which are used  

1. clone - Used to clone a repo from github. To do this, we use the http key from the repo  
    git clone https://github.com/Sckarge/Git_practice.git    
2. status - To check the status of changed and untracked files in your local.  
    git status  
3. add - Used to track yet untracked files in git(use . instead of file name for all files to be tracked)  
We can also add remote before add to connect to a git repo if we did not clone  
    git add .  
    git add index.html  
    git remote add origin  https://github.com/Sckarge/new_git.git  
4. commit - Changes are commmitted to local. Done before pushing  
    -m can be added for Title the first time and description the second time  
5. git push - Can be used to push to a remote repo. Requires repo link and branch the first time.  
    If -u (upstream) is used, we can use it without the parameters(This is done by default if the repo is cloned)  
    git push  
    git push -u origin master  
6. remote - Used with -v to get all remote repos attached  
    git remote -v

## Branching

We use branches as a sort of sandbox to test our changes before pushing them to the master branch

7. branch - to check all the branches (* will be present in front of current branch)  
    Can be used with -d to delete a branch(to be used after a merge)
    git branch  
    git branch -d feature-branch-1  
8. checkout - Used to switch to a branch, but, also to create branches using -b  
    git branch -b feature-branch-1  
9. diff - to check the differences b/w your current branch and another branch(also shows unstaged changes)  
    git diff master  
10. pull - Used to pull a branch from github to local. This can be done after some changes have been made to that branch that we need to make in our local.  
    git pull (after upstream has been set)

## Merge

When we merging two branches, we may have some merge conflicts, these need to be resolved manually.  

11. merge - merges the branch mentioned into our current branch  
    git merge master(In case of conflicts solve in code editor)
    We then need to commit the changes  
NOTE: This merges into your current branch not master

## Undoing in git  
In git,we can undo add and commits, in the following ways-

12. reset - Used to reset changes
    git reset (resets last add)
    git reset HEAD~1 (used to change the header position at the last commit)
    git reset --hard deb4165278cf252d8509613f7d23feab7cdbe5f6
    (removes all changes with --hard, hash obtained from log)  
13. log - log of all commits with their hashes
    git log