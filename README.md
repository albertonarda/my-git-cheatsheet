# My GIT Cheatsheet

## Update username and email
`git config --global user.name "John Doe"`

`git config --global user.email "john@doe.org"`

## Update credential
To update your credentials, go to Control Panel -> Credential Manager -> Generic Credentials

## Update remote branch list
`git remote update origin --prune`

## Add existing project to a repository
`git init`

`git add .`

`git commit -m "First commit"`

`git remote add origin <remote-repository-URL>`

`git remote -v`

`git push -u origin master`

`# the remote repository must be empty`
