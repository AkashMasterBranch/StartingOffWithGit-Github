# StartingOffWithGit-Github
Documenting git and github setup

[To determine what licence to use for your code](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/licensing-a-repository)
(Guide to determine license may be added in future revisions)
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