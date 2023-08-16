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