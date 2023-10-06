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
git push origin master (origin represents the location of Git repository in the local system)




