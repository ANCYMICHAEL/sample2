# Git and GitHub Notes (VS Code)

## Step 1: Add Git Account to VS Code

1. Install Git on your computer.
2. Open VS Code.
3. Open Terminal → Select Git Bash.
4. Configure your GitHub account:

```bash
git config --global user.name "Your Username"
git config --global user.email "your_email@example.com"
```
## Basic Git Commands


| Command                   | Description                                                      |
| ------------------------- | ---------------------------------------------------------------- |
| `git status`              | Shows the current status of files (modified, staged, untracked). |
| `git init`                | Creates a new Git repository in the current folder.              |
| `git add filename`        | Adds a specific file to the staging area.                        |
| `git add .`               | Adds all files to the staging area.                              |
| `git commit -m "message"` | Saves a snapshot of staged changes with a message.               |
| `git checkout commit_id`  | Moves to a specific commit (detached HEAD state).                |
| `git switch -`            | Switches back to the previous branch.                            |
| `git checkout master`     | Switches to the master/main branch.                              |

---


### 1. git status

Checks the current state of files in the repository.

```bash
git status
```

### 2. git init

Creates a new local Git repository.

```bash
git init
```

### 3. git add filename

Adds a file to the staging area.

```bash
git add filename
```

Example:

```bash
git add index.html
```

### 4. git commit -m "message"

Saves staged changes as a commit.

```bash
git commit -m "added file"
```

### 5. git checkout commitid

Moves to a specific commit.

```bash
git checkout commitid
```

### 6. git switch - / git checkout master

Returns to the previous branch or switches to the master/main branch.

```bash
git switch -
```

or

```bash
git checkout master
```

---

## Branch Management

# Branch Commands

| Command            | Description                               |
| ------------------ | ----------------------------------------- |
| `git branch`       | Lists all branches.                       |
| `git branch dev`   | Creates a new branch named `dev`.         |
| `git checkout dev` | Switches to the `dev` branch.             |
| `git switch dev`   | Modern way to switch to the `dev` branch. |

---

### 7. git branch

Displays all available branches.

```bash
git branch
```

### 8. git branch dev

Creates a new branch named dev.

```bash
git branch dev
```

### 9. git checkout dev

Switches to the dev branch.

```bash
git checkout dev
```

---

## GitHub Commands

### 10. git clone URL

Downloads a GitHub repository to your local computer.

```bash
git clone URL
```

### 11. git push

Uploads local commits to GitHub.

```bash
git push origin main
```

---
# GitHub Commands

| Command                | Description                                               |
| ---------------------- | --------------------------------------------------------- |
| `git clone URL`        | Downloads an existing GitHub repository to your computer. |
| `git push origin main` | Uploads local commits to GitHub.                          |
| `git pull origin main` | Downloads and merges the latest changes from GitHub.      |

---


## GitHub Concepts

### 12. Fork

A **Fork** creates your own copy of someone else's GitHub repository under your GitHub account.
### 13. Pull Request (PR)

A **Pull Request** is a request to merge your changes into another branch or repository after review.
---

# Git Workflow Stages

Working Directory
↓
git add
↓
Staging Area/Edit Files
↓
git commit -m "message"
↓
Local Repository
↓
git push
↓
GitHub Remote Repository


Description:

• Working Directory – Files you edit in VS Code.
• Staging Area – Files selected for the next commit.
• Local Repository – Commits stored on your computer.
• Remote Repository (GitHub) – Online copy of your project.
• Push – Sends local commits to GitHub.
• Pull – Downloads updates from GitHub.
