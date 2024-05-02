---
title: Git, Commands Cheat Sheet
date: 2024-04-25 13:00:00 +800
categories: Git
author: Clark
math: true
mermaid: true
comments: true
---
<!-- markdownlint-capture -->
<!-- markdownlint-disable -->
# Glossary 
1. **Git**: A distributed version control system designed for tracking changes in source code during software development
2. **Repository(repo)**:A data structure that stores metadata and objects for a Git Project, includes files, commit history, branches, and configuration settings
3. **Commit**: A snapshot of changes made to files in a repository at a specific point in time. 
4. **Staging**: Preparing files before being committed to the repository. Staged files are the ones ready to be included in the next Commit
5. **Branch**: A branch allows developers to work on separate features or fixes in a parallel manner without affecting the main code base
6. **Push**: the action of uploading local commits from your local repository to a remote repository such as GitHub or GitLab or your own or your company's hosted repositories. 
7. **Pull**: The action of fetching the changes from a remote repository and merging them with your local repository.
8. **Merge**: The process of integrating changes from one branch into another branch
9. **Conflict**: A situation where Git cannot automatically merge changes from different branches due to conflicting modifications to the same file.
10. **Clone**: The action of creating a local copy of a remote repository to your machine


---
# COMMONLY USED COMMANDS
```bash
git clone [url]
```
Retrieve an entire repository from a remote/hosted location via URL

```bash
git status
```

Show which files are modified, untracked or staged commit.

```bash
git add [file] 
git add .
```

Adds the changes in a specific file(add `[file]`) or all modified files(add .) in the working directory or the staging area, preparing them for the next commit.

```bash
git commit -m "[commit message]"
```

Commits the staged changes to the local repository with a descriptive commit message explaining the changes made

```bash
git push
```

Pushes the committed changes from your local repository to the remote repository, keeping them synchronized.

```bash
git pull
```

Fetches changes from the remote repository and merges them to your local repository

```bash
git checkout [branch name]
```

Switches to the specific branch.

```bash
git merge [branch name]
```

Merges changes from the specified branch into the current branch

```bash
git log
```

Displays a chronological list of commits in the repository along with the messages, authors, timestamps, and commit IDs.


<!-- markdownlint-restore -->

---


source: github.com
# SETUP & INIT

```bash
git config --global user.name "[firstname lastname]"
```

set a name that is identifiable for credit when review version history \

```bash
git config --global user.email "[valid-email]"
```

set an email address that will be associated with each history maker

```bash
git config --global color.ui auto
```

set automatic command line coloring for Git for easy reviewing

```bash
git init
```

initialize an existing directory as a Git repository

```bash
git clone [url]
```

retrieve an entire repository from a remote/hosted location via URL

# STAGE & SNAPSHOT
```bash
git status
```

