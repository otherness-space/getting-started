# Git commands I use most

## New local directory
`cd /Users/user-dir/Documents/dir/dir/../`

`git init`

Confirm there is at least one file, empty or not. I usually install a `README.md` and `LICENSE.md` from a stock blank.
```
LaptopNames-MBP:getting-started laptop-name$ ls

LICENSE.md	README.md
```
`git add . `

`git commit -m 'First commit'`

`git remote add origin git@github.com:user-name/repo-name.git`

`git remote -v`

`git push origin master`
```
git init ; git add . ; git commit -m 'First commit' ; git remote add origin git@github.com:user-name/repo-name.git ; git remote -v ; git push origin master
```


## Add new file
`git add . ; git commit -m 'MUST INCLUDE COMMIT MESSAGE' ; git push origin --all ; git status ; git branch ; git diff`

`git add . ; git commit -m '' ; git push origin --all ; git status ; git branch ; git diff`


## File changes
`git commit -a -m 'MUST INCLUDE COMMIT MESSAGE' ; git push origin --all ; git status ; git branch ; git diff`

`git commit -a -m '' ; git push origin --all ; git status ; git branch ; git diff`


## These commands provide information
`git status`

`git diff`

`git branch`

`git remote`

`git remote -v`

`git remote show origin`

`git log --oneline --decorate`

`git log --oneline --decorate --graph --all`

`git status ; git diff`


## Create and select a branch
`git branch [branch name]`

`git checkout [branch name]`


## Combines the previous two
`git checkout -b [branch name]`

`git checkout -b [] ; git status ; git branch ; git diff`


## Merge obviously
`git merge [branch name]`

`git checkout master ; git status ; git branch ; git diff; [branch-name]; git status ; git branch ; git diff; `


## Stage and commit
`git add . `

`git commit -m 'Narrative'`


## Combines the previous It does't work on a new file addition, just on file changes, in my experience
`git commit -a -m 'Narrative'`


## Delete branch
`git branch -d [branch name]`


## Upload to the GitHub
`git push origin master`

`git push origin [branch name]`

`git push origin --all`


## Clone and remote
Execute `cd` to appropriate directory

`git clone git@github.com:user-name/repo-name.git`

`git remote add [remote-alias] git@github.com:user-name/repo-name.git`

`git remote rm [remote-alias]`

`git fetch [remote-alias]`
