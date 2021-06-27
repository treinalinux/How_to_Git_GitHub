# How_to_Git_GitHub

## Pattern Commits

Before starting with git try to follow a **pattern for your commits**.

Think that the organization you are going to work with must follow a pattern, and that is why it is interesting that you follow some pattern, i recommend using the **Conventional Commits**.

### [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/)

A specification for adding human and machine readable meaning to commit messages


```
<type>[optional scope]: <description>

[optional body]

[optional footer(s)]
```

The commit contains the following structural elements, to communicate intent to the consumers of your library:

1. **fix**: a commit of the type fix patches a bug in your codebase (this correlates with PATCH in Semantic Versioning).

2. **feat**: a commit of the type feat introduces a new feature to the codebase (this correlates with MINOR in Semantic Versioning).

3. **BREAKING CHANGE**: a commit that has a footer BREAKING CHANGE:, or appends a ! after the type/scope, introduces a breaking API change (correlating with MAJOR in Semantic Versioning). A BREAKING CHANGE can be part of commits of any type.

4. **types other than fix**: and feat: are allowed, for example @commitlint/config-conventional (based on the the Angular convention) recommends build:, chore:, ci:, docs:, style:, refactor:, perf:, test:, and others.

5. **footers other than BREAKING CHANGE**: <description> may be provided and follow a convention similar to git trailer format.

Additional types are not mandated by the Conventional Commits specification, and have no implicit effect in Semantic Versioning (unless they include a BREAKING CHANGE). A scope may be provided to a commit’s type, to provide additional contextual information and is contained within parenthesis, e.g., feat(parser): add ability to parse arrays.

#### Exemples
```
###
feat: allow provided config object to extend other configs

###
refactor!: drop support for Node 6

###
refactor!: drop support for Node 6

BREAKING CHANGE: refactor to use JavaScript features not available in Node 6.

###
docs: correct spelling of CHANGELOG

###
feat(lang): add polish language
```

**Original Source: View list full**

- [Conventional Commits - EN](https://www.conventionalcommits.org/en/v1.0.0/)
- [Conventional Commits - PT-BR](https://www.conventionalcommits.org/pt-br/v1.0.0/)


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

## Logs

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

## Stash

```
git add .

git stash

git stash list

# apply return dot on project
git stash apply

# clear the list on stash
git stash clear

# Prefer to use pop instead of apply
# pop bounces and cleans old stash

git stash pop
```
