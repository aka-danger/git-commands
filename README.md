# git-commands
Useful git commands for those weird situations

## Login
- Username: `git config --global user.name "aka-danger" `
- Password: `git config --global user.email "email@example.com" `

##Proxy
- `git config --global http.proxy http://student no:password@10.200.254.1:3128`

## List global variables
- `git config --global --list`

## unset global variables
- `git --config --global --unset-all variable.name`
- `git --config --global --unset variable.name`

## Deleting files from folder instead of git 
- `git ls-files --deleted -z | xargs -0 git rm`

## How to make your branch the master
- `git checkout branch-name`
- `git merge -s ours master`
- `git checkout master`
- `git merge branch-name`

##how to move changes from one branch to another 
###example if you are working on master by mistake and want the changes in another branch
- `git stash`
- `git checkout <existing branch>`
- `git stash pop`

## Revert changes to modified files.
- `git reset --hard`

## Remove all untracked files and directories. 
### (`-f` is `force`, `-d` is `remove directories`)
- `git clean -fd`

## Discard unstaged files
- `git checkout -- *`
