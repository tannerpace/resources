# Helpful Commands 

## PM2
```
pm2 restart index 
```
--restarts server useful after pulling in changes from git












## Git

###  

```
`git add` .
```

### 2.
```
`git commit -m "message"  .
``` 

### 3. 
```
git push
```
### 4. 
```
git pull origin master
```

### 5.
```
git status
```

### 6. 
```
git log
```

### 7. 
```
git checkout -b branch_name
```

### 8. 
```
git checkout branch_name
```

### 9. 
```
git branch
```

### 10. 
```
git branch -d branch_name
```

### 11. 
```
git merge branch_name
```

### 12. 
```
git remote add origin
```

### 13. 
```
git remote -v
```

### 14. `git remote rm origin`

### 15. `git remote set-url origin`

### 16. `git clone`

### 17. `git reset --hard`

> is used to reset the local repository to the state of the remote repository. This is useful when you have made changes to the local repository that you want to discard.

### 18. `git remote update origin --prune`

> deletes all the remote-tracking references that no longer exist on the remote. This is useful when you have deleted a branch on the remote and want to remove the corresponding reference locally.

### 19. `git reset --hard origin/master`

> this command will reset your local branch to match the remote branch. This is useful when you have made changes to the local repository that you want to discard.

### 20. `git reset --hard HEAD~1`

> this command will reset your local branch to the previous commit. This is useful when you have made changes to the local repository that you want to discard.

## NODE VERSION MANAGER

###1 `node -v > .nvmrc`

> this command will create a .nvmrc file with the current version of node installed on your machine.
> ###2 `nvm use`
> this command will use the version of node specified in the .nvmrc file.
> ###3 `nvm install 16`
> this command will install the version of node specified ie 16
> ###4 `nvm alias default 16`
> this command will set the default version of node to 16

# 1. `git add` .

# 2. `git commit -m "message`

# 3.`git push origin master`

# 4. `git pull origin master`

# 5.`git status`

# 6. `git log`

# 7. `git checkout -b branch_name`

# 8. `git checkout branch_name`

# 9. `git branch`

# 10. `git branch -d branch_name`

# 11. `git merge branch_name`

# 12. `git remote add origin`

# 13. `git remote -v`

# 14. `git remote rm origin`

# 15. `git remote set-url origin`

# 16. `git clone`

# 17. `git reset --hard`

is used to reset the local repository to the state of the remote repository. This is useful when you have made changes to the local repository that you want to discard.

# 18. git remote update origin --prune

deletes all the remote-tracking references that no longer exist on the remote. This is useful when you have deleted a branch on the remote and want to remove the corresponding reference locally.

# 19. `git reset --hard origin/master`

this command will reset your local branch to match the remote branch. This is useful when you have made changes to the local repository that you want to discard.

# 20. `git reset --hard HEAD~1`

this command will reset your local branch to the previous commit. This is useful when you have made changes to the local repository that you want to discard.

# 21. `git reset --hard HEAD~2`

this command will reset your local branch to the previous two commits. This is useful when you have made changes to the local repository that you want to discard.

# 22. `git reset --hard HEAD~3`

this command will reset your local branch to the previous three commits. This is useful when you have made changes to the local repository that you want to discard.

# 23. `git reset --hard HEAD~4`

this command will reset your local branch to the previous four commits. This is useful when you have made changes to the local repository that you want to discard.

# 24. `git reset --hard HEAD~5`

this command will reset your local branch to the previous five commits. This is useful when you have made changes to the local repository that you want to discard.

# 25. `git init`

this command will initialize a local git repository. This is useful when you want to start tracking a local project with git.

# 26. `git worktree add -b branch_name`

this command will create a new branch and switch to it. This is useful when you want to create a new branch and switch to it.

# 27. `git diff`

. This command will show you the differences between the files in your working directory and the files in your staging area. This is useful when you want to see what changes you have made but have not yet committed.

# 28. `git diff --staged`

this command will show the differences between the index and the last commit. This is useful when you want to see what changes you have made.

# 29. `git diff branch_name`

this command will show the differences between the working directory and the specified branch. This is useful when you want to see what changes you have made.

# 30. `git diff branch_name --staged`

this command will show the differences between the index and the specified branch. This is useful when you want to see what changes you have made.

# NODE VERSION MANAGER

#1 `node -v > .nvmrc`
this command will create a .nvmrc file with the current version of node installed on your machine.

#2 `nvm use`
this command will use the version of node specified in the .nvmrc file.

#3 `nvm install`
this command will install the version of node specified in the .nvmrc file.

#4 `nvm install --lts`
this command will install the latest version of node.

#5 `nvm install --lts --reinstall-packages-from=system`
this command will install the latest version of node and reinstall all the packages from the system.

# mysql
You can update root password anytime from MySQL shell.
$ mysql -uroot -p
mysql> ALTER USER 'root'@'localhost' IDENTIFIED BY 'MyNewStrongP@ssw0d!';

login with root user 
mysql -u root -p

###General
lsof -i :5001.  -kill proccess on a port


#github credintal helper cmds
  git status
  gh auth login
  sudo snap install gh
  gh auth login
  git pull
  gh auth login
  git config --global user.email
  git config --global myemail@gmail.com
  git config --global user.email myemail@gmail.com
  




steps to set up ssl
assuming your ec2 is up and responding to http on /
first create a target group this should connect to the ec/
define a security group that will accept all https traffic on the port your ec2 is on   
define a security group that will accept traffic from the alb security group
create an application load balancer
confirm that its target group is the one with the ec2 set up any health checks as needed
health checks should be on http port 80

----no this looks wrong-----confirm that alb has a listner on the same port as ec2 and that it is https
alb listener should be on https and port 443---- think this was my mistake
regester a domain with route  53 this will be needed to get a ssl certificate 
point the domain at the alb
add the ssl for domain to the alb

