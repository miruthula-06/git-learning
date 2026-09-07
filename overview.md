GIT-LEARNING-COMMANDS

Git and Github
Git-version control system
Github-Online platform 

What is git?
It is version control system and it can help you easily track changes on your project and it is called as DVCS
For example Today develop a index.html that work correctly tomorrow we have add extra features/correction update now we have bug/error will be shown, so we have git means you can go back to previous version easily

What is DVCS?
Git is distributed version control system,because every developer we can have complete copy of project including history also

What is Github?
It is online platform where you can store, share your project and collaborate with other developers work on same project

What is repo?
Repo means that will be main project files and history

Git command

We creating new project that in your local machine that connect git(local) to github(remote/online) means we have use this commands

git init-we are create a git repo(local folder create .git file that maintain commit,branch,history)
git add .-Add this file for staging area
git commit - “new file”-Save the file for local repo(Git)
git branch -M <branch-name> - Rename the current branch name
git remote add origin URL - connect git(local repo) to github(online repo)
git push origin main - Push the project git into github

Already existing repo in git(local-machine) you have to connect github means use this command

git remote add origin URL - connect git(local repo) to github(online repo)
git branch -M <branch-name> - Rename the current branch name
git push origin main - Push the project git into github


Branch All Commands
Create branch
git branch <branch-name> - create branch
git switch/checkout -c <branch name> - create new branch and switch that branch

View Branch list
git branch - show only local branch
git branch -r - show only github branch
git branch -a -show git + github branch

Branch switch and moving
git switch/checkout <branch-name> -current branch switch to another branch
git switch -  this command in current branch I am there means back to previous branch

Rename the branch
git branch -M <new-branch-name> -rename the branch
Git branch -m <old-name> <new-name> -rename the specific branch 

Delete branch
git branch -d <branch-name>

Merge branch
Git merge <source-branch> - Merges changes from <source-branch> into your currently active branch
For example 
You standing on main branch means that is target branch and merge the login branch means that is source branch

Setup & Configuration 

git config --global user.name "Miruthula" - set your name
git config --global user.email "your@email.com" - set your email address
(Without global means it applies only to the current repository.)
git init - Initializes a new local Git repository in your current folder 
git clone URL-Downloads an existing repository from github

git status-Shows tracked, untracked files
git add <file>-Stages a specific file for the next commit 
git add . - Stages all new, modified, and deleted files in the directory 
git diff - 
(For ex previously <h1>Hello</h1> then <h1>Hello Miruthula</h1> But you haven't run git add . then run git diff means git show me removed and added changes)
 

git diff  - -staged
(same example but one correction you have to change then run this command git add . and git diff command show me staged files)

git pull - Gets the latest changes from GitHub and applies them to your current branch. 
git fetch - Gets the latest changes from GitHub and do not apply them to your current branch and check
git log - see your commit history
git stash - You changed some code, but you don't want to commit it now.Git temporarily saves your changes. 
git stash pop -  you changed some code then save it and bring your changes back