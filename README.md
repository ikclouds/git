# git

- [git](#git)
  - [Install git](#install-git)
  - [Git initial configuration](#git-initial-configuration)
  - [Get help](#get-help)
  - [Clone repository](#clone-repository)
  - [Commit, pull, push](#commit-pull-push)
  - [Information sources](#information-sources)

## Install git

```bash
# Ubuntu
sudo apt install git

# RHEL
sudo dnf install git-all

# Windows
choco install git  # run as Administrator

git --version
```

## Git initial configuration

```bash
# Show origin configuration

git config --list --show-origin

# List current configuration

git config --list --system  # /etc/gitconfig
git config --list --global  # ~/.gitconfig , ~/.config/git/config
git config --list --local   # ./git/config

# Add initial configuration

git config --global user.name "ikclouds"
git config --global user.email "<ikclouds91@gmail.com>"
git config --list --show-origin

# git config --global core.editor vim
# git config --global core.editor "'C:/Program Files/Notepad++/notepad++.exe' -multiInst -notabbar -nosession -noPlugin"
```

## Get help

```bash
git help config
git config --help
git config -h
```

## Clone repository

```bash
git clone git@github.com>:ikclouds/git.git
git clone git@github.com:ikclouds/repo.git
git clone https://github.com/ikclouds/git.git

cd git
git status
```

## Commit, pull, push

```bash
# Change project folder
cd git

# Get git working area status
git status -h
git status -s
git status

# List branches (main)
git branch
git branch -l  # --list
git branch -a  # --all

# Add all files to the index/stage area
git add .
git add index.html
git add -A
git add -u
# 
git commit -m "add commit doc" 
# or 
# git commit -a -m "add commit doc"

# Incorporates changes from a remote repository into the current branch
git pull

# Updates remote refs using local refs, while sending objects to the remote repository
git push
```

## Information sources

- Documentation
  - Book
    - [1.6 Getting Started - First-Time Git Setup](https://git-scm.com/book/ms/v2/Getting-Started-First-Time-Git-Setup)
