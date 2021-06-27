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
