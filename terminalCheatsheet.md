# Terminal Cheatsheet
## Overview
This Cheatsheet provides a quick overview of all the terminal commands learnt during the BNTA course so far. This includes navigation, file/folder editing, and github basics!

**Tip:** *For a quick way to get into the Terminal on Mac, do cmd + space to openm Spotlight, then type in 'Terminal'*


## Inspecting your File System

- `pwd`   = Print working directory. Gives you the pathway to your current working directory *e.g /Users/leilapeltier/Documents*

- `ls`    = lists all files and folders in the current working directory
- `ls -a` = lists all files and folders - including **hidden** files such as git files

- `ls -l`  = lists of files and folders - including extras like permissions, owner, file size and date last modified
- `ls -al` = same as above but including those **hidden** files 😉


## Navigating Your File System

- `cd` + folder_name  =  Change directory. *e.g. `cd Documents` would move you into the Documents folder* If you just type `cd` + enter it would move you to your home directory - quick and easy way to get back to the beginning!

- `cd ~` = Takes you back to your home directory - quick and easy way to get back to the beginning! You can also just type `cd` on its own for the same effect!

**Tip:** An easy way to know if you are in the home directory is if you see the blue `~` symbol!

- `cd -`  = Takes you to the directory you were just in - kinda like an 'undo' of sorts.
- `cd ..` = Takes you to the directory above the one you are currently in *e.g. if you were currently in `e.g /Users/leilapeltier/Documents/bnta_work/week01` this would take you to the `bnta_work folder` , and then if you did the command again it would take you to the `Documents` folder and so on!

## Opening Files

- `open` + file/folder_name = Opens the named file/folder. For folders this will open in the corresponding GUI - ie. Finder on Mac or Windows Explorer on PC. For files this will be in the default app for the file type.

**Tip:** You can open files using specific programs by using the appropriate keyword, defined within the program. e.g. To open a file in the VSCode editor, use `code my_file.txt`.

## Manipulating Files and Folders

- `mkdir` + folder_name        = Make Directory. Creates a new folder
- `touch` +file_name.extension = Creates a new file. *e.g. `touch my_picture.png` would create a png file called `my_picture`, `touch my_powerpoint_presentation.pptx` a powerpoint file, and so on*

- `rm` + filename = **Permanently** deletes named file
- `rm -r` + folder_name = **Permanently** deletes named directory


- `mv` + old_name + new_name = Renames a file or folder **e.g. `mv my_file.txt my_new_filename.txt`
- `mv` + file/folder + directory path = Moves file/folder to named directory e.g. `mv test_folder /Users/leilapeltier/Documents/`. It is VERY important you do filepath instead of just the name of the folder/file! If you don't you might just accidentally rename it instead!


- `cp` + filename + destination pathway    = Copies named file into named directory
- `cp -r` foldername + destination pathway = Copies named folder into named directory - including subfolders!
- `code` = 

### (Extras/Shortcuts)

- `..` = Shortcut for ' directory above this one'. 
- `.`  = Shortcut for 'this directory'. Good for if you want to do things like copy everything in a current directory into another, open everything in the current directory etc. without typing in a whole filepath.

- `mkdir` + folder1 + folder2 + folder3 = Creates multiple folders in the current directory at the same time. The same principle works for other similar commands such as `touch`, `rm`, `cp` etc.
- When renaming a file you can change the file type at the same time *e.g. `mv my_file.txt my_new_photo.png`*

## Git Commands

The following is everything you can do locally:

- `git init` = Initialises (aka sets up) Git in the current directory. You will know Git has been set up in terminal as the directory name will be followed by `git` and the branch type in brackets.

- `git status` or `gst` = Tells you the status of the files in the current directory, including: which files are being tracked, which have been modified, and what files have been staged.

- `git add` + folder_path/filename = Stages a specific directory or file.
- `git add .` = Stages all files in the directory - including ones beginning with a dot.
- `git add --all` = Stages all files in the directory - including ones beginning with a dot AND deletes files not in the current working tree.
- `git commit -m` + "commit message" = Commits changes that have been staged. Commit message is used to let future you and others know what exaclty changed in that commit *e.g. `git commit -m"added a missing link to homepage"`*

- `git revert` + repo ID = Reverses changes made in a specified commit
- `git reset` + repo ID = Reverses changes made in a specific commit and all commits after it (keeping the histroy still though)
- `git rebase` + repo ID = Same as git revert but also deletes the history of the commit too.

The following is everything related to pushing and pulling between local and online repository:

- `git remote add` + origin + your_url = Uploads your local repo to Github.
-`git clone` repository_url = Gets a copy of a GitHub repository on your local device.
- `git push` + origin + branch_type = Uploads changes made in local repo to the online repo. *e.g. ` git push origin main`
- `git pull` + origin + branch_type = Downloads changes someone else has made on GitHub *e.g. `git pull origin main`*




