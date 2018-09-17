# Git Commands


Git Command | Description
------------|------------
git init | Creates a new Git repository
git add filename | Add the file to staging index
git status | List all new or modified files to be committed
git log | Show committed files
git log --oneline | 
git ls-tree <given tree: like master> | List the contents of a given tree object, like Hash Value
**git reset --option** | Move the HEAD.
git reset --soft (hash value) | Reset the place of HEAD pointer. Does not touch the index file or the working tree at all. Also, move the files (after new HEAD pointer place) from repo to staging index. 
git reset --mixed (hash value) | Reset the place of HEAD pointer. **Resets the index but not the working tree** (i.e., the changed files are preserved but not marked for commit) and reports what has not been updated.
git reset --hard (hash value)
git reset HEAD <filename> | Unstage the file


