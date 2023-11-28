Using Git on GitHub
If you find yourself stuck in the list view, SHIFT + G to jump the end of the list, then q to exit the view.


Git is a version control system, used for:
Tracking code changes
Tracking who made changes
Coding collaboration



Why Git?
Over 70% of developers use Git!
Developers can work together from anywhere in the world.
Developers can see the full history of the project.
Developers can revert to earlier versions of a project.



What does Git do?
Manage projects with Repositories
Clone a project to work on a local copy
Control and track changes with Staging and Committing
Branch and Merge to allow for work on different parts and versions of a project
Pull the latest version of the project to a local copy
Push local updates to the main project



Working with Git
Initialize Git on a folder, making it a Repository
Git now creates a hidden folder to keep track of changes in that folder
When a file is changed, added or deleted, it is considered modified
You select the modified files you want to Stage
The Staged files are Committed, which prompts Git to store a permanent snapshot of the files
Git allows you to see the full history of every commit.
You can revert back to any previous commit.
Git does not store a separate copy of every file in every commit, but keeps track of changes made in each commit!


What is GitHub?
Git is not the same as GitHub.
GitHub makes tools that use Git.
GitHub is the largest host of source code in the world
In this tutorial, we will focus on using Git with GitHub.


Git Install
https://git-scm.com/


Check version 
git --version


Configure Git
git config --global user.name "mslamwing"
git config --global user.email "mslamwing@gmail.com"

Note: Use global to set the username and e-mail for every repository
For just the current repo, remove global


Creating Git Folder

mkdir myproject // makes a new directory
cd myproject


Go back to previous folder
cd .. 


Initialize Git
git init 


To initialize a folder as a Git repository, you would use the git init command within that folder. This command creates a hidden subfolder within the folder named .git that contains all the necessary metadata for version control.
Git creates a hidden folder to keep track of changes.
Initializing a folder, in the context of version control with Git, means creating a new Git repository. Here's why it's necessary:
Version Control: Initializing a repository in a folder starts version control for that folder's content, allowing you to track changes, revert to previous states, branch out, and more.


Collaboration: It sets up the necessary framework for collaborating with others. Each participant can have their version of the project, which can later be merged.


Change Tracking: It allows you to keep an historical record of all the changes made to the files in the repository. Every commit records a snapshot of the files, who made changes, and a message describing the change.


Branching and Merging: Git repositories facilitate branching and merging, enabling you to work on different features or experiments in isolation and then combine them when ready.


Remote Repositories: By initializing a local repository, you set the stage to connect to a remote repository (like on GitHub, GitLab, Bitbucket), which is crucial for backup, sharing, and remote collaboration.


To create a file in a folder
touch index.html




Put coding inside the folder
nano index.html





list the files in our current working directory
ls


check the Git status
git status
git status
On branch master

No commits yet

Untracked files:
  (use "git add ..." to include in what will be committed)
    index.html
Now Git is aware of the file, but has not added it to our repository!
Files in your Git repository folder can be in one of 2 states:
Tracked - files that Git knows about and are added to the repository
Untracked - files that are in your working directory, but not added to the repository
When you first add files to an empty repository, they are all untracked. 
To get Git to track them, you need to stage them, or add them to the staging environment.
We will cover the staging environment in the next chapter.



Git Staging Environment
Staged files are files that are ready to be committed to the repository/a collection of files you are working on.




add it to the Staging Environment. So The file should be Staged.
git add index.html







add all files in the current directory to the Staging Environment
Using --all instead of individual filenames will stage all changes (new, modified, and deleted) files.


git add --all
git add -A



Since we have finished our work, we are ready move from stage to commit for our repo.
Adding commits keep track of our progress and changes as we work. Git considers each commit change point or "save point". It is a point in the project you can go back to if you find a bug, or want to make a change.
When we commit, we should always include a message.
By adding clear messages to each commit, it is easy for yourself (and others) to see what has changed and when.


Git Commit
//-m: Specify Commit Message
git commit -m "First release of Hello World!"





Git Help
Git —-help
Git commit —-help
git command -help -  See all the available options for the specific command
git help --all -  See all possible commands







To view the history of commits for a repository, you can use the log command:
Git Commit Log




