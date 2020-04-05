# 4 Git Storage
1. Working directory
2. Index
3. Repository
4. Stash

# Working Directory --> Index --> Repository

#Moving data to the Right
##1. Moving data from Working Directory to Index
git add filename  
git diff -> view different between working dir and index  
git status  

##2. Moving data from index to repostory
git commit -m "Commit message"  
git diff --cached --> view different between index and repository  
git status  

##3. Moving data from local repository to remote repository
git push  

# View branch
git branch

# view different between branch lisa and master
git diff lisa master

# Switch to branch 'lisa'
git checkout lisa

# Remove data from index
1. git rm --cached filename
2. rm filename

# Rename Files from menu.txt to menu.md
1. rm menu.txt menu.md
2. git add menu.md
3. git add menu.txt

# Rename file from menu.md to menu.txt using git mv
1. git mv menu.md menu.txt

