
## During development
### git pull(=git fetch + git merge)
Pull often to make sure you have the latest updates from other feature branches to avoid possible merging conflicts after merging
### git add filename (git add .)
Add untracked files and stage changes. Don't Use add .  could be risky
### git commit -m "message of desciption on this commit"
Do commits often to record every change you made
### git push 
Will update and build on remote so be careful


## Remove added files:
### git rm --cached filename

## Checkout on last commits
### git reset --soft
Keep working dir changes and staged changes, back to last commit
### git reset --mix
Keep working dir changes, unstage staged changes to working dir, back to last commit
### git reset --hard
Back to last commit, remove all changes

## Temporarily Wipe changes before commiting file changes (both staged and unstaged files)
### git stash save "message" ("git stash list" to check stash history)
Save stashes and work on sth else
The stash is local to your Git repository; stashes are not transferred to the server when you push.
## git stash pop stashname("git stash list" to find stash name if having multiple stashes)
Remove your latest stash (cut from stash history, won't kept there) and copy onto your working environment
Go back to your uncommited work
## git stash apply
Reapply the changes to your working copy and keep them in your stash
## git stash branch newbranchname stashname
Create a new branch on stash to avoid conflicts

## View difference between two commits
### git diff commit1code commit2code (eg.HEAD: LAST COMMIT)
Will show changes of commit2 comparing to commit1

## Merge feature branch into master
### git checkout master
### git merge featurebranchname

## Creating tags for special events (version releases)
### git tag -a tagname(eg. v1.0) -m "Release 1.0"
