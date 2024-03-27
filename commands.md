## Setup

```
git config --global user.name "[firstname lastname]" 
```
set git name
```
git config --global user.email "[valid-email]" 
```
set git email
```
git config --global color.ui auto
```
set cmd line coloring

## Init

``` 
git init
```
initialize an existing directory as a Git repository 
``` 
git clone [url]
```
retrieve an entire repository

## Stage and Snapshot

```
git status 
```
shows modified files
```
git add [file]
```
add a file to next commit
```
git reset [file]
```
unstage and reset changes of file
``` 
git diff
```
show what is changed
```
git diff --staged 
```
show what is staged not committed
``` 
git commit -m "[descriptive message]" 
```
commit the changes

## Branch and Merge

```
git branch
```
list branches
```
git branch [branch-name]
```
create a new branch
```
git checkout 
```
switch to another branch
```
git merge [branch]
```
merge the specific branch
```
git log
```
show all commits 

## Inspect and Compare

``` 
git log
```
show commit history
``` 
git log branchB..branchA 
```
compare commits in one branch
``` 
git merge [alias]/[branch]
```
remote branch to current
``` 
git push [alias] [branch]
```
commits to remote repository branch
``` 
git pull 
```
fetch and merge any commits

## Tracking Path Changes

``` 
git rm [file] 
```
delete file from project
``` 
git mv [existing-path] [new-path]
```
change existing file path
``` 
git log --stat -M
```
show all commits and movement

## Rewriting History

``` 
git rebase [branch]
```
keep main branch up to date while resetting the progress of the other branch
``` 
git reset --hard [commit]
```
reset branch to specific state

## Ignoring Patterns

```
logs/
*.notes
pattern*/
```
desired patterns
```
git config --global core.excludesfile [file]
```
system wide ignore pattern

## Temporary Commits

``` 
git stash 
```
save modified and staged changes
``` 
git stash list
```
list of stashed items
``` 
git stash pop
```
write on top of the stash
``` 
git stash drop
```
discard changes on top of the stash