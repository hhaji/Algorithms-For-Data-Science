# Git Cheat Sheet & Useful Facts About Git


Git Commands  | Description
--------------|------------
git init | Create a new Git repository
git config --global user.name "name" | Sets the name you want to attach to your commit transactions 
git config --global user.email "email address" | Sets the email you want to attach to your commit transactions 
git config --global alias.arbitrary_name "command name" | Change the "command name" to arbitrary_name
git config --global core.editor "editor_name" | Set up your editor to "editor_name", e.g., "nano", "vim", etc. 
git add "file_name" | Add the file to staging index
git add . | Add all files from working directory to staging index
git status | List all new or modified files to be committed
git commit -m "message" | Add files from staging index to repository committed by the "message"
git commit --amend -m "new_message" | Change the commit message by using the amend flag
git log | Show committed files
git log --oneline | List one commit per line and it shows the first 7 characters of the hash value and the commit message.
git diff | View difference between staging index and working directory
git diff "hash values" | Show changes between the working tree and the index or a tree, changes between the index and a tree, changes between two trees, or changes between two files on disk
git diff --staged | View difference between HEAD and staging index
git diff HEAD | View difference between HEAD and working directory
git diff --color--words branch1..branch2 | Show differences between branch1 and branch2 using color fonts
git branch "branch_name" | Create a branch whose name is "branch_name"
git branch --m "old_name" "new_name" | Change the old name of the branch to new one 
git branch --d "branch_name" | Delete the branch
git branch | List branches
git branch -m "new" | Rename current branch to "new"
git checkout -b "branch_name" | Create the branch and switch to this branch
git checkout "branch_name" | Switch to "branch_name"
git checkout remotes/origin/"branch_name" | Switch to a remote "branch_name"
git checkout -- "file_name" | Discrad changes in the working directory
git checkout "hash value" | Switch to a specific commit (determined by hash value)
git merge "branch_name" | Incorporate changes from the named commits (since the time their histories diverged from the current branch) into the current branch
git ls-tree "branch_name" | List the contents of "branch_name", like hash Value
git reset --soft "hash value" | Reset the place of HEAD pointer. Does not touch the index file or the working tree at all. Also, move the files (after new HEAD pointer place) from repo to staging index
git reset --mixed "hash value" | Reset the place of HEAD pointer. Reset the index but not the working tree (i.e., the changed files are preserved but not marked for commit) and reports what has not been updated
git reset --hard "hash value" | Make your current branch (typically master ) back to point at hash value and make the files in your working tree and staging index the same as the versions committed in the has value
git reset HEAD "file_name" | Unstage "file_name"
git reset HEAD^ | Pop your last commit out of the history
git tag | List all tags
git remote -v | List the URL of the remote repo
git remote add origin "URL"  | Associate your repo with remote 
git remote set-url origin "URL" | Update an existing remote
git push -u origin "branch_name" | Push "branch_name" to remote
git pull origin "branch_name" | Pull the most recent changes from that remote branch
git clone "URL" | Copy a repo from URL
git revert HEAD | Revert the previous commit
git submodule add URL/User_name/module_repo name_repo | Add an existing Git repo (module_repo) of a user (User_name) as a submodule of the repo that you are working on
<br>

# Aliases

Alias | Code (Should be Run in Terminal) | Description
------|----------------------------------|------------
git logg | git config --global alias.logg "log --graph --decorate --oneline --abbrev-commit --all" | Display a graphic and readable log on one line using various colours

# Setup a Git credential helper
Rather than entering your GitHub username and password every time you push, you can setup a Git credential helper to manage this for you.

OS | Command 
---|--------
MAC | git config --global credential.helper osxkeychain
Linux | git config --global credential.helper 'cache --timeout=3600'

Once a credential helper is enabled, the next time you git push, you will add your credentials to the helper.



