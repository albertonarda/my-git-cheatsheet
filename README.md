# My GIT Cheatsheet

## Update username and email
`git config --global user.name "John Doe"`

`git config --global user.email "john@doe.org"`

## Use Window Credential Manager

`git config --global credential.helper manager`

## Update credential with Window Credential Manager
To update your credentials, go to Control Panel -> Credential Manager -> Generic Credentials

## Update remote branch list
`git remote update origin --prune`

## Tree view
`gitk --all`

## Add existing project to a repository
`git init`

`git add .`

`git commit -m "First commit"`

`git remote add origin <remote-repository-URL>`

`git remote -v`

`git push -u origin master`

`# the remote repository must be empty`

## Rebase
`git checkout experiment`

`git rebase master`

## Change remote URL
`git remote set-url origin git@github.com:USERNAME/REPOSITORY.git`

## Go to particular commit
`git log --abbrev-commit --pretty=oneline`

copy the hash

`git reset --hard HASH`

## Go back to the most recent commit

`git checkout master`

`git pull`

## Add/stage all files

`git add .`

## View staged files

`git diff --name-only --cached`

## Un-stage all files

`git reset`
