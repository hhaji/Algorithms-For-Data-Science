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
git ls-tree branch-name | List the contents of the branch, like hash Value
git reset --soft (hash value) | Reset the place of HEAD pointer. Does not touch the index file or the working tree at all. Also, move the files (after new HEAD pointer place) from repo to staging index. 
git reset --mixed (hash value) | Reset the place of HEAD pointer. **Resets the index but not the working tree** (i.e., the changed files are preserved but not marked for commit) and reports what has not been updated.
git reset --hard (hash value) | Make your current branch (typically master ) back to point at hash value and make the files in your working tree and staging index the same as the versions committed in the has value.
git reset HEAD <filename> | Unstage the file


