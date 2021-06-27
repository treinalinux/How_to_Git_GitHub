# How_to_Git_GitHub


## Start project local

```
git init
```

## Clone project remote

```
git clone git@github.com:treinalinux/How_to_Git_GitHub.git
```

## Add project remote

```
git remote add git@github.com:treinalinux/How_to_Git_GitHub.git
```

### View remote repository details

```
git remote -v
```

## Config of git

- local  - Only project local
- global - All projects of user current
- system - All users of computer

Prefer modify config global of user current

### set editor default

Case use vim

```
git config --global core.editor vim

```

Case use vscode

```
git config --global core.editor code

```

### Editing and listing the configs

```
git config --global --edit

git config --global --list
```

## Commits

### Status

```
git status

git status -s
```

### Add files

```
git add Gemfile

# need to run from root
git add .

## can use in any dir of project
git add --all

```

### Commits

```
commit -m "How use git: First commit"

## useful when you need to set the last commit information
git commit --amend --no-edit

```

### Logs

```
git log

git log --oneline

# Cutom
git log --pretty=format:'%C(blue)%h%C(yellow)%d %C(green)%cr %C(cyan)%cn %C(white)%s'
```

## Grep
```
git shortlog -s --grep rails
```
