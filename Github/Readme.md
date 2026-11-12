# GitHub

## 1. Introduction
GitHub is an online platform used to host Git repositories and collaborate on software projects.

**Git vs GitHub:**
- Git tracks changes in files.
- GitHub hosts repositories and supports collaboration.

## 2. Creating a Repository
1. Sign in to [GitHub](https://github.com/).
2. Select **New repository**.
3. Enter a repository name.
4. Choose Public or Private visibility.
5. Click **Create repository**.

- **Public:** Anyone can view the repository.
- **Private:** Only authorized users can access it.

## 3. README File
A `README.md` file introduces the project and explains its purpose, features, installation, and usage.

Example:
```markdown
# Calculator
A simple Python calculator.

## Features
- Addition
- Subtraction
```

## 4. Connecting Local Repository to GitHub
Add a remote repository:
```bash
git remote add origin REPOSITORY_URL
```

Check remote connections:
```bash
git remote -v
```

## 5. Pushing Code to GitHub
Upload local commits to GitHub:
```bash
git branch -M main
git push -u origin main
```

## 6. Cloning a Repository
Cloning creates a local copy of a remote repository.

```bash
git clone REPOSITORY_URL
```

## 7. Fetching and Pulling Changes

| Command | Purpose |
|---|---|
| `git fetch origin` | Downloads remote updates |
| `git pull` | Downloads and integrates updates |
| `git push` | Uploads local commits |

## 8. Branches
A branch is an independent line of development used to work on features without directly changing the main branch.

```bash
git branch
git branch feature-login
git switch feature-login
git switch -c feature-login
```

Merge a branch:
```bash
git switch main
git merge feature-login
```

## 9. Pull Requests
A Pull Request (PR) proposes changes for review and merging into another branch.

Steps:
1. Push the feature branch to GitHub.
2. Open a Pull Request.
3. Request reviews.
4. Address feedback.
5. Merge the approved changes.

## 10. Forking
A fork creates a separate copy of another user's repository under your account. It allows you to work independently and propose changes through Pull Requests.

## 11. GitHub Features
- **Issues:** Track bugs, tasks, and feature requests.
- **Projects:** Organize tasks and monitor progress.
- **Code Review:** Review and improve code.
- **Releases:** Publish specific project versions.

## 12. Best Practices
- Write clear commit messages.
- Use meaningful branch names.
- Review code before merging.
- Keep README files updated.
- Never upload passwords or secret keys.

## Conclusion
GitHub makes it easier to host projects, collaborate with developers, and manage software development.