# Git

## 1. Introduction
Git is a **distributed version control system** used to track changes in files and manage projects.

## 2. Types of Version Control Systems
- **Local VCS:** Tracks changes on a local computer.
- **Centralized VCS:** Uses a central server (e.g., SVN).
- **Distributed VCS:** Every user has a local copy of the repository (e.g., Git).

## 3. Installing Git
- Windows: Download from [git-scm.com](https://git-scm.com/).
- Ubuntu: `sudo apt install git`
- macOS: `brew install git`

Check installation:
```bash
git --version
```

## 4. Configuring Git
```bash
git config --global user.name "Student Name"
git config --global user.email "student@example.com"
git config --global --list
```

## 5. Creating a Repository
```bash
mkdir my-project
cd my-project
git init
```
`git init` initializes a Git repository and creates a hidden `.git` directory.

## 6. Three Main Areas of Git
- **Working Directory:** Where files are created or modified.
- **Staging Area:** Holds changes selected for the next commit.
- **Repository:** Stores committed changes and history.

## 7. Basic Git Commands

| Command | Purpose |
|---|---|
| `git status` | Check file status |
| `git add filename` | Stage a file |
| `git add .` | Stage all changes |
| `git commit -m "message"` | Save changes |
| `git log` | View commit history |
| `git log --oneline` | View short commit history |
| `git diff` | Compare unstaged changes |
| `git diff --staged` | Compare staged changes |
| `git ls-files` | List tracked files |

## 8. Ignoring Files
Create a `.gitignore` file to exclude files from tracking.

Example:
```text
__pycache__/
*.pyc
.env
*.log
```

## 9. Renaming and Deleting Files
```bash
git mv old.py new.py
git rm old.py
```

## 10. Restoring and Reverting Changes

Unstage a file:
```bash
git restore --staged main.py
```

Discard unstaged changes:
```bash
git restore main.py
```

Revert a commit:
```bash
git revert COMMIT_ID
```
Revert creates a new commit that undoes an earlier commit.

## 11. Best Practices
- Write meaningful commit messages.
- Commit changes regularly.
- Check status before committing.
- Use `.gitignore` for unnecessary files.

## Conclusion
Git helps track changes, maintain project history, and manage code efficiently.