# My GIT Cheatsheet

## Update username and email

```zsh
git config --global user.name "John Doe"
git config --global user.email "john@doe.org"
```

## Update remote branch list

```zsh
git remote update origin --prune
```

## Delete remote branch

```zsh
git push -d <remote_name> <branchname>
```

Note: In most cases, <remote_name> will be origin.

## Tree view

```zsh
gitk --all
```

## Add existing project to a repository

```sh
git init
git add .
git commit -m "First commit"
git remote add origin <remote-repository-URL>
git remote -v
git push -u origin master
# the remote repository must be empty
```

## Rebase

```sh
git checkout experiment
git rebase master
```

## View Remote Repository

```sh
git remote -v
```

## Change remote URL

```sh
git remote set-url origin git@github.com:USERNAME/REPOSITORY.git
```

## Go to particular commit

```sh
git log --abbrev-commit --pretty=oneline
```

copy the hash

```sh
git reset --hard HASH
```

## Go back to the most recent commit

```sh
git checkout master
git pull
```

## Add/stage all files

```sh
git add .
```

## View staged files

```sh
git diff --name-only --cached
```

## Un-stage all files

```sh
git reset
```

## Use Window Credential Manager

```sh
git config --global credential.helper manager
```

## Update credential with Window Credential Manager

To update your credentials, go to Control Panel -> Credential Manager -> Generic Credentials
