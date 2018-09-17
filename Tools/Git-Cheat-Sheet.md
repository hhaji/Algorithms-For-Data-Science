# Git Commands


Git Command | Description
------------|------------
git reset --soft (hash value) | Reset the place of HEAD pointer. Does not touch the index file or the working tree at all. Also, move the files (after new HEAD pointer place) from repo to staging index. 
git reset --mixed (hash value) | Reset the place of HEAD pointer. Resets the index but not the working tree (i.e., the changed files are preserved but not marked for commit) and reports what has not been updated.

