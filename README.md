# 4 Git Storage
1. Working directory
2. Index
3. Repository
4. Stash

# Working Directory --> Index --> Repository

# Moving data to the Right
## 1. Moving data from Working Directory to Index
> git add filename  
> git diff
view different between working dir and index  
> git status  

## 2. Moving data from index to repostory
> git commit -m "Commit message"  
> git diff --cached 
view different between index and repository  
> git status  

## 3. Moving data from local repository to remote repository
> git push  

# View branch
> git branch

# view different between branch lisa and master
> git diff lisa master

# Switch to branch 'lisa'
> git checkout lisa

# Remove data from index
> git rm --cached filename
>
> rm filename

# Rename Files from menu.txt to menu.md
> rm menu.txt menu.md
>
> git add menu.md
>
> git add menu.txt

# Rename file from menu.md to menu.txt using git mv
> git mv menu.md menu.txt

# Git use SHA-1 
> git cat-file -p master   
> tree 6cbc48cf00a9624a2cc43f6d88fba2be0ed9dbd8  
> parent 9c63593b06cc9331eedbcc7e503ef1aa96724f6a  
> author sandyverden <sandyverden@gmail.com> 1586099087 +0700  
> committer sandyverden <sandyverden@gmail.com> 1586099087 +0700  
> rename to README.d  

## Describe SHA tree 
> git cat-file -p 6cbc48cf00a9624a2cc43f6d88fba2be0ed9dbd8  
> 100644 blob def3e5bfebc06f2f77d55b9fbb098522101098a4    README.md  
> 100644 blob 3dff7cd890f0adf75fe98e8513df416cf38ee931    menu.txt  
> 040000 tree 5ac651563e6b6cd406fe095903dab7fc5c7135ae    recipes  

## Describe SHA blob
> git cat-file -p 3dff7cd890f0adf75fe98e8513df416cf38ee931  
> Spaghetti alla Carbonara  
> Apple Pie  
> Cheesecake  
> Chicken Tikka Masala  
> Nasi Goreng  
> mie goreng  

# Git Merge from branch 'sandi-dev' to branch 'master'
>  git merge sandi-dev

# Change branch from branch 'master' to branch 'sandi-dev'
> git checkout sandi-dev
