# GIT
### GIT Tutorial Udemy [Link](https://www.udemy.com/course/git-complete/)

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

git commit -am "<note>": add and commit

git push : up files in Local Repository(.git) to remote repository area ( GitHub ) 

git mv <source> <destination> :  Move or rename a file, a directory, or a symlink

git rm <file> : Remove files from the working tree and from the index

git restore <file> : to discard changes in working directory

git restore --staged <file>: to unstage

git reset HEAD^ : Bach to before commit 

git reflog : show all log git

git reset (id commit/HEAD@{index}) : Go to commit or commit have HEAD@{index}
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

git diff <branch local A> <branch local B>: show changes between branch A and branch B
```

## Command git branch
```git
git branch: show all branch local

git branch -a: show all branch local and remote

git branch <name branch>: add new branch to local

git checkout <name branch>: change new branch

git branch -m <name old branch> <name new branch> : change name branch

git branch -d <name branch>: delete branch

git branch -b <name new branch>: create new branch and checkout to new branch
``` 


## Command git merge
```git
git merge <branch A>: merge code in branch A to branch here

if branch here dont have commit => fast forward

git merge <branch A> --no-ff: disable fast forward merge

## after conflic
git merge --continue: to continue after resolving conflicts in a failed merge

git merge --abort: Abort the current conflict resolution process, and try to reconstruct the pre-merge state. If an autostash entry is present, apply it to the worktree.

git merge --quit: Forget about the current merge in progress. Leave the index and the working tree as-is. If MERGE_AUTOSTASH is present, the stash entry will be saved to the stash list.
``` 


## Command git rebasing
```git 
git rebase <branch A>: Here to branch A

git rebase --about: check out the original branch and stop rebasing 

git rebase --continue: resolved this problem go next step

git rebase --skip: prefer to skip this patch

``` 

## Command git stashing
```git 
git stash : move all changes in file (old) to other memory

git stash -u : move all changes in file (old and new) to other memory

git stash apply: merge new stash from other memory in here

git stash apply stash@{<index>}: merge stash(index) from other memory in here

git stash list: get list stash in other memory

git stash drop: drop new stash

git stash drop stash@{<index>}: drop stash(index) 

git stash pop : the same 'git stash apply' + 'git stash drop'

git stash save "<message>": config name to stash this is happy if have multiple stashes

git stash show stash@{<index>}: show file change in stash

git stash clear: remove all stashes

git stash branch <name new branch>: move all change of stash old branch to new branch
``` 


## Command git tagging
```git 
git tag <tag name> : create new tag

git tag --list: get all tag

git show <tagName>: show document pin to tag

git tag --delete <tag name>: delete tag

git tag -a <tag name> : annotated tags

git diff <tag 1> <tag 2>: compare between tag 1 and tag 2

git tag <tag name> <id commit>: add tag to commit

git tag <tag name exit> -f <id commit> :update tag 

git push --tags: upload all tag to remote

git push <tag name>: upload tag to remote

git push :<tag name> : delete tag in remote
``` 

## Command git cherry pick
```git 
git cherry-pick <id commit>: add commit with id to branch here ( creat new commit before add to branch here)


## after conflic
git cherry-pick --continue : to continue after resolving conflicts in a failed cherry-pick or revert.

git cherry-pick --skip: Skip the current commit and continue with the rest of the sequence.

git cherry-pick --abort: Cancel the operation and return to the pre-sequence state.

git cherry-pick --quit: Forget about the current operation in progress. Can be used to clear the sequencer state after a failed cherry-pick or revert.
``` 

### if conflic. After resolve you should add file in working tree before command continue

