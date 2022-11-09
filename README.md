# Commands Used Daily
## Git
### 1. `git add` .
### 2. `git commit -m "message`
### 3.`git push origin master`
### 4. `git pull origin master`
### 5.`git status`
### 6. `git log`
### 7. `git checkout -b branch_name`
### 8. `git checkout branch_name`
### 9. `git branch`
### 10. `git branch -d branch_name`
### 11. `git merge branch_name`
### 12. `git remote add origin`
### 13. `git remote -v`
### 14. `git remote rm origin`
### 15. `git remote set-url origin`
### 16. `git clone`
### 17. `git reset --hard`
>is used to reset the local repository to the state of the remote repository. This is useful when you have made changes to the local repository that you want to discard.
#### 18. `git remote update origin --prune`
>deletes all the remote-tracking references that no longer exist on the remote. This is useful when you have deleted a branch on the remote and want to remove the corresponding reference locally.
#### 19. `git reset --hard origin/master`
>this command will reset your local branch to match the remote branch. This is useful when you have made changes to the local repository that you want to discard.
#### 20. `git reset --hard HEAD~1`
>this command will reset your local branch to the previous commit. This is useful when you have made changes to the local repository that you want to discard.

## NODE VERSION MANAGER
####1 `node -v > .nvmrc`
>this command will create a .nvmrc file with the current version of node installed on your machine.
###2 `nvm use`
>this command will use the version of node specified in the .nvmrc file.

###3 `nvm install 16`
this command will install the version of node specified ie 16
