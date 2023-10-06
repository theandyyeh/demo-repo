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

