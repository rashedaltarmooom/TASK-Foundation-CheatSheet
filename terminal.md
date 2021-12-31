# Terminal & Github cheatsheet

## Terminal basic commands

`cd <FOLDER_NAME>`: is used to navigate to the folder
`cd ..`: is used to go up in a directory level
`cd -`: is used to go back in history
`cd `: is used to go to home directory `~`
`cd ~`: is used to go to home directory `~`
`cd /`: is used to go to root directory `/`

`ls`: is used to list all items in a folder
`ls -la`: is used to list all items in a folder with details and hidden folder

`pwd`: is used to print the current working directory to know where we are in the folder structure

`touch` is used to create a new file
`mkdir` is used to create a new directory
`nano <fileName>` is used to open a text editor to edit a file
`code .` to open Vs code for the current working directory
`rm <FILE>` to remove a single file
`rm -rf` to force remove a whole folder with its whole content

## Github basics

**Fork**
to fork any repository, you just have to click on the right side button that has the `FORK` label on it, and you should double check that you forked by checking the user name in the link if it has your username.

## Git terminal basic commands

`git clone <REPO_LINK>`: is used to clone a repository given a specific link

`git status`: is used after every git command we do to get the status of the git repository

`git add .`: is the first step to be able to commit and push a git repository. We should add all file in the working directory to **staging** status by using the dot `.` notation

`git commit -m "MESSAGE"`: is used to **commit** the files, and save their history. You can only use this command if you have staged the files using the `git add` command.
If you do not add a message, you will open a VIM editor.
`git commit` -> open vim.
To quit vim, you use the command

1. Escape
2. type: `:q`

`git push`: is used to **push** the files if you are authorized to push.

> **COMMON MISTAKE!**
> If you didn't fork a repo, and you cloned it and you tried to push, it will not let you push, because you don't own the repo.
