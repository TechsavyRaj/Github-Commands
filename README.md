# Git Commands Cheat Sheet

A simple list of useful Git commands that developers commonly use :-

## Table of Contents

- [Basic Commands](#basic-commands)
- [Working with Commits](#working-with-commits)
- [Branching](#branching)
- [Stashing](#stashing)
- [Remote Repositories](#remote-repositories)
- [Undoing Changes](#undoing-changes)
- [Tags](#tags)
- [Collaborating](#collaborating)
- [Advanced Commands](#advanced-commands)
- [Cheatsheet Translations](#translations)

---

## Basic Commands

| Command               | Description                              |
|-----------------------|------------------------------------------|
| `git init`            | Initialize a new Git repository.        |
| `git clone <url>`     | Clone an existing repository.           |
| `git status`          | Show the working directory status.      |
| `git log`             | Show the commit history.                |
| `git show <commit>`   | Show details of a specific commit.      |

---

## Working with Commits

| Command                       | Description                                   |
|-------------------------------|-----------------------------------------------|
| `git add <file>`              | Add a file to the staging area.              |
| `git add .`                   | Add all changes to the staging area.         |
| `git commit -m "message"`     | Commit changes with a message.               |
| `git commit --amend`          | Amend the previous commit.                   |
| `git reset <file>`            | Unstage a file.                              |
| `git reset --hard <commit>`   | Reset to a specific commit, discarding changes. |

---

## Branching

| Command                        | Description                                  |
|--------------------------------|----------------------------------------------|
| `git branch`                   | List all branches.                          |
| `git branch <branch-name>`     | Create a new branch.                        |
| `git branch -d <branch-name>`  | Delete a branch.                            |
| `git checkout <branch-name>`   | Switch to a branch.                         |
| `git checkout -b <branch-name>`| Create and switch to a new branch.          |
| `git merge <branch-name>`      | Merge a branch into the current branch.     |
| `git merge --squash <branch-name>`| Squash multiple commits into one during branch merge. |

---

## Stashing

| Command                  | Description                                   |
|--------------------------|-----------------------------------------------|
| `git stash`              | Save uncommitted changes for later use.      |
| `git stash push -m <message>`| Save uncommitted changes with message.   |
| `git stash list`         | List all stashes.                            |
| `git stash apply`        | Apply the most recent stash.                 |
| `git stash apply <stash>`| Apply a specific stash.                      |
| `git stash pop`          | Apply the most recent stash & removes it from stash list. |
| `git stash pop <stash>`  | Apply a specific stash & removes it from stash list. |
| `git stash drop`         | Delete a specific stash.                     |

---

## Remote Repositories

| Command                                   | Description                                   |
|-------------------------------------------|-----------------------------------------------|
| `git remote -v`                           | Show remote repositories.                    |
| `git remote add <name> <url>`             | Add a new remote repository.                 |
| `git fetch <remote>`                      | Fetch changes from a remote repository.      |
| `git pull <remote> <branch>`              | Pull changes from a remote branch.           |
| `git push <remote> <branch>`              | Push changes to a remote branch.             |
| `git push --set-upstream <remote> <branch>` | Push a branch and set upstream tracking.    |

---

## Undoing Changes

| Command                        | Description                                   |
|--------------------------------|-----------------------------------------------|
| `git checkout -- <file>`       | Discard changes to a file.                   |
| `git revert <commit>`          | Revert a specific commit.                    |
| `git reset <commit>`           | Undo commits, keeping changes in the working directory. |
| `git reset --hard`             | Undo all changes and commits permanently.    |

---

## Tags

| Command                    | Description                                   |
|----------------------------|-----------------------------------------------|
| `git tag`                  | List all tags.                               |
| `git tag <tag-name>`       | Create a new tag.                            |
| `git tag -d <tag-name>`    | Delete a tag.                                |
| `git push <remote> <tag>`  | Push a tag to a remote repository.           |
| `git push --tags`          | Push all tags to a remote repository.        |

---

## Collaborating

| Command                             | Description                                   |
|-------------------------------------|-----------------------------------------------|
| `git pull`                          | Fetch and merge changes from a remote branch. |
| `git fetch`                         | Fetch changes from a remote repository.      |
| `git rebase <branch>`               | Reapply commits on top of another branch.    |
| `git cherry-pick <commit>`          | Apply a specific commit to the current branch. |
| `git blame <file>`                  | Show who modified each line of a file.       |

---

## Advanced Commands

| Command                        | Description                                   |
|--------------------------------|-----------------------------------------------|
| `git diff`                     | Show changes between commits, branches, or working directory. |
| `git reflog`                   | Show the history of all actions (including resets). |
| `git config --global <key> <value>` | Configure Git settings globally.          |
| `git submodule add <url>`      | Add a submodule to the repository.           |
| `git bisect`                   | Use binary search to find the commit that introduced a bug. |

---

## Translations

- [English](README.md)
- [Español](README.es.md)
- [Française](README.fr.md)
- [Português](README.pt.md)
- [Türkçe](README.tr.md)
- [日本語](README.jp.md)
- [हिन्दी](README.hi.md)
