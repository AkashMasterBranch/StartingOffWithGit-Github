# StartingOffWithGit-Github
Documenting git and github setup

[To determine what licence to use for your code](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/licensing-a-repository)
------------------------------------------------------------------------------------------------------------------
Git needs to be installed and ready (I am using Gitbash with windows)

To set up a project with git, we need to first initialize configuration variables to get credit for changes. 

Within Git, 

> git config --global user.name "Akash Patel"
> git config --global user.email "email@email.com"

Make sure to use Github or Gitlab email address. Change email if necessary for different projects. 

Next, create a folder on your PC to store project files. Navigate to this directory in Git by using 

> cd c:/users/andthenwhereveritslocated

Use "dir" to see the files in the directory if you need to. Alternatively, use ls -la to see the file names of all files along with their permissions and including hidden files starting with a period. 

Next, use "git init" to manage projects in the folder of the directory you are in. Git will now store information about the project here. 

You can use "cd" with just the name of the file to move into this directory or use "cd .." to move to previous directory. 

--------------------------------------------------------------------------------------------------------------------------
Staging Environment is a temporary area to store files we may want to commit later on. 
To move a file to staging, 
> git add FILENAME

Alternatively, can add all files using one of the following
> git add --all
> git add -A

Or, you can refer to current directory using the following
> git add .

To finally commit, use
> git commit -m "First Commit"

To see what git has kept track of so far, use "git log" 
"git status" lets you see what changed in your clone's current branch before commiting. 

- git push :  Updates github with new code changes from your clone (from git to github) - own branch
- git pull :  Updates clone with new code changes from github (from github to git) - own branch
- git fetch: Updates clone with new branches (from github to git) - clone knows about other branches
- git merge [branch_name]: Combines code from any branch and your current branch (in git or github)
  - harder to fix merge conflicts on github

- git clone [github repo url]:     create a local clone of the github repo in your local computer
- git remote -v:                   this will tell you what .git servers (or mirrors) your clone is using. The origin one is what your clone was created from
- git remote add [remote variable] [server url]: this is for if your clone is using multiple servers. You can have one clone update multiple github repositories.
- git add [file_name(s)]:          adds new files to track in current git branch
- git add -u [file_name(s)]:       updates tracked files to be committed in current git branch
- git checkout [file_name(s)]:     undo all changes from the specified file
- git commit -m "[commit message]": create a commit for your current branch with a commit message (each commit has a unique commit id)
- git checkout -b [branch_name]:   create a new branch based on the current branch you are on
- git checkout -t [branch_name]:   change to a new branch you haven't been on before in your local clone (only need to do this first time only)
- git checkout [branch_name]:      switch to a branch that is already existing on your local clone
- git checkout [commit_id]:        switch to an older version of your current branch based on your commit history from git log
- git checkout HEAD:               go back to your current version of your branch
- git reset HEAD:                  undo a git add if you accidentally add files or changes you do not want to commit
- git revert [commit id]:          undo a commit that was made in your current branch
- git stash:                       save off changes without adding or commiting on your local clone before switching to a new branch (for code you're not ready to commit)
- **git stash pop:**                   recover and get back the saved off changes in the branch you ran the git stash command on
- 
