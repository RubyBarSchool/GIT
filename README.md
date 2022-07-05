# GIT
### GIT Tutorial Udemy [Link](https://fpt-software.udemy.com/course/git-complete/)

<img src="./image/git-life-cycle.png" alt="GIT life cycle" >

Command List

```git
#Basic command os
pwd : show path directory

mkdir <name folder> : create new folder

cd <name/path> : go to path folder

rm <file> : remove file

rm -r <dir> delete directory dir last directory

#Basic command git
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

git log : show list commit log

git log -- <file> : show log of file

git log --since="3 days ago" : show log in 3 last day

git log --all --graph --decorate --oneline: show log commit and show graph and show imple commit

# Git alias
# Config 
git config --global alias.<name alias> "<cmd>"
example: git config --global alias.showloggraph "log --all --graph --decorate --oneline"

git showloggraph = git log --all --graph --decorate --oneline

git diff : Show changes between commits, commit and working tree, etc

git diff HEAD : show changes between working directory and loca repository
```
