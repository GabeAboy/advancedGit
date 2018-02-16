### advancedGit
## Common commands
    - git init                 - git status
    - git add < file file > .  - git branch
    - git checkout < > -(b)    - git log
    - git commit -m ''
    - git push
## Need to know commands and what they do
# ~ tilda
  **Unstaging changed**
    `$ git reset HEAD < file >`
    `$ git reset HEAD .` 
    `$ git unstage .`
  **Undoing commits**
    `$ git reset --soft HEAD~1`
        This command will reset the local repository to point to the last commit, and put those changes back into staging
    `$ git reset --hard HEAD~1`
        Will completely delete the commit and throw away any changes
  **Store current work with un-tracked files**
    `$ git stash -u`
    `$ git stash list`
  **Bring stashed work back to the working directory**
    `$ git stash pop`
  **Saving the origin to push**
    `$ git push --set-upstream origin <branch>`
    `$ git push`
  **Fetching changes upstream**
   `$ git fetch upstream`
        Or exclude the upstream
  **Removing a files from the working index** 
    `$ git rm --cached <>`
  **To delete a file (force)**
    `$ git rm -f <>`
  **To remove an entire directory**
    `$ git rm -r <>`
  **Search the working directory for anything**
    `$ git grep "<CONTENT>"`
  **Squashing commits**
    `$ git rebase -i HEAD~4`
    Squashing puts all last 4 commits into one commit. While doing this I have to use the interactive mode in vim :wq to get out 
  **Git rebase**
    `$ git fetch origin`
    `$ git rebase origin/feature`
    Rebase is a way to rewrite history, by stacking commits on top of pushed commits
    `$ git rebase -i HEAD~1`
  **Deleting a branch**
    `$ git branch -d <localBranch>`
  
  **Vim notes**
    Exit program: esc :wq
    Interactive mode : i
