# Git Cheat Sheet


Git Command | Description
------------|------------
git init | Create a new Git repository
git add filename | Add the file to staging index
git add . | Add all files from working directory to staging index
git status | List all new or modified files to be committed
git commit -m "message" | Add files from staging index to repository committed by the "message"
git log | Show committed files
git log --oneline | List one commit per line and it shows the first 7 characters of the hash value and the commit message.
git diff (hash values) | Show changes between the working tree and the index or a tree, changes between the index and a tree, changes between two trees, or changes between two files on disk
git diff --color--words branch1..branch2| Show differences from branch1 to branch2 using color fonts
git branch branch-name | Create a branch whose name is branch-name
git checkout branch-name | switch to branch-name
git checkout -- filename | Discrad changes in the working directory
git branch | List branches
git ls-tree branch-name | List the contents of branch-name, like hash Value
git reset --soft (hash value) | Reset the place of HEAD pointer. Does not touch the index file or the working tree at all. Also, move the files (after new HEAD pointer place) from repo to staging index
git reset --mixed (hash value) | Reset the place of HEAD pointer. **Resets the index but not the working tree** (i.e., the changed files are preserved but not marked for commit) and reports what has not been updated
git reset --hard (hash value) | Make your current branch (typically master ) back to point at hash value and make the files in your working tree and staging index the same as the versions committed in the has value
git reset HEAD <filename> | Unstage the file


