# GIT
### GIT Tutorial Udemy [Link](https://fpt-software.udemy.com/course/git-complete/)

<img src="./image/git-life-cycle.png" alt="GIT life cycle" >

## Command List

## Basic command os
```git
pwd : show path directory

mkdir <name folder> : create new folder

cd <name/path> : go to path folder

rm <file> : remove file

rm -r <dir> delete directory dir last directory
```

## Basic command git
```git
git version: check git version

git config --global <>: config environment global

git clone <link remote repository>: clone repository project in GitHub to Local

ls: show anything in path

git status: check status files in path

git add <file/files/.>: add or change file in Local Area to Stagging Area

git commit -m "<note>": add  or changr file in Stagging Area to Local Repository Area (.git)

git push : up files in Local Repository(.git) to remote repository area ( GitHub ) 

git mv <source> <destination> :  Move or rename a file, a directory, or a symlink

git rm <file> : Remove files from the working tree and from the index
```
## Command git log
```git
git log : show list commit log

git log -- <file> : show log of file

git log --since="3 days ago" : show log in 3 last day

git log --all --graph --decorate --oneline: show log commit and show graph and show imple commit

# Git alias
# Config 
git config --global alias.<name alias> "<cmd>"
example: git config --global alias.showloggraph "log --all --graph --decorate --oneline"

git showloggraph = git log --all --graph --decorate --oneline
```

## Command git diff
```git
git diff : Show changes between commits, commit and working tree, etc

git diff HEAD : show changes between working directory and loca repository

git diff --staged HEAD: show changes between stagging area and local repository

git diff -- <file> : show changes in file

git diff <id commit 1> <id commit 2>: show changes between 2 commits

git diff HEAD ^HEAD: show changes between git repository at HEAD and git repository at 1 commit before HEAD

git diff <branch main local> origin/<branch main remote>: show changes between git local and git remote
```

## Command git branch
```git
git branch -a: show all branch local and remote

git branch <name branch>: add new branch to local

git checkout <name branch>: change new branch

git branch -m <name old branch> <name new branch> : change name branch

git branch -d <name branch>: delete branch

``` 
