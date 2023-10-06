# Demo Title

Some description!

# Install Git
Mac: Git should've been installed. 
Terminal: 
git --version

# Visual Studio Code
Explorer(folder) -> open a folder called "git" 

# Pull the Repo created before from Github to the local system (using Visual Studio Code, a type of code editor)
VSC -> View -> Terminal
It shows "git" automatically because the folder name is "git." To input command lines, you still need to type git...... on your own. 
Go to Github, and copy the line from "Clone" (Code -> Local -> SSH -> copy the key) (if not having SSH key, you need to generate one in the local system and add one to your account)
git clone git@github.com:theandyyeh/demo-repo.git (this is to pull the repo from Github)
cd demo_repo (this is to change the directory of Visual Studio Code into demo_repo) (BTW, underscore will be replaced by hyphen in VSC)
ls -la (list all the folders, including directory and hidden folders) (can also be written as "la" only) (those hidden folders you saw are the files that saved your commits, which means they are for version control)

## This is a subheader

# Track your updates
git status (shows all the files that are created, updated, and deleted)

add a new file on VSC under demo_repo, called index.html
put <div> Hello! </div> in it.

git status (again) (you will find out index.html has not been trackded, so we need to tell Git to track it)
git add . (. is a regular expression, meaning to check all the things above, in both untracked and modified sections)
git add index.html (alternatively, you can specify them individually)
clear (used to clear the command lines above to make the terminal interface clearer)
git status (check again, and they should be tracked)

# Commit those updates
git commit -m "this is the title" -m "this is for description box. this means message you want to leave, and supposedly, it should state what and why behind the commits you are making."

# So far it's still only saved locally. We need to "push" it to Github. (if you haven't got your SSH key set up, you should do it beforehand so that GitHub recognizes your local system)
git push origin main (origin represents the location of Git repository in the local system; master is the thing in your Github which is the destination; in my case, it's main rather than master)

# Start a demo_repo_2 from the local system!
create one directly on VSC
cd ../demo-repo-2 (go into the folder; if you want to go into a directory or file, then use cd __ directly)
create README.md
git init (this is to put the new repo into the Git Repository because originally this was not there!)
git status
git add .
git push origin main (ERROR)(fatal: 'origin' does not appear to be a git repository fatal: Could not read from remote repository.) (it's because demo-repo-2 was NOT CLONED from the hub!!!!)
Go to GitHub and create a NEW repository (named the same as this one)
Copy the SSH url
git remote add origin git@github.com:theandyyeh/demo_repo_2.git (remote means...somewhere else but not this computer)
git remote -v (shows all the repository connected to the current repo)
git push origin main (NOW it works!!!)

If you are LAZY, you can do...
git push -u origin main (-u means upstream, so in the future, it knows what you want to do)
git push (this will be the code you can use in the future)

# This header will ONLY be in the branch....




