# Git_How_To

Hi This is GIT about Git 
Here are the basic instruction HOW TO uppload , etc...

Tady je základní **How-To Guide** pro práci s Git, napsaný v **Markdown** formátu. Tento text můžete použít ve svém projektu nebo repozitáři jako základní přehled práce s Git.

```markdown
# Git Basics: How-To Guide

This guide provides essential Git commands and workflows to help you manage your projects efficiently.

---

## 1. Initial Setup

Before using Git, you need to set your username and email:

```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

Check your Git configuration:

```bash
git config --list
```

---

## 2. Starting a New Repository

### Initialize a Git repository in your project folder:
```bash
git init
```

### Add all files to the staging area:
```bash
git add .
```

### Commit the changes:
```bash
git commit -m "Initial commit"
```

---

## 3. Working with an Existing Repository

### Clone a repository:
```bash
git clone https://github.com/username/repository-name.git
```

### Check the current status of the repository:
```bash
git status
```

### Pull the latest changes from the remote repository:
```bash
git pull origin main
```

---

## 4. Making Changes

### Add specific files to the staging area:
```bash
git add file_name
```

### Add all modified files:
```bash
git add .
```

### Commit the changes with a message:
```bash
git commit -m "Your commit message"
```

---

## 5. Working with Remote Repositories

### Add a remote repository:
```bash
git remote add origin https://github.com/username/repository-name.git
```

### Push changes to the remote repository:
```bash
git push origin main
```

### Pull changes from the remote repository:
```bash
git pull origin main
```

---

## 6. Branching

### Create a new branch:
```bash
git branch branch_name
```

### Switch to the new branch:
```bash
git checkout branch_name
```

### Create and switch to a branch in one command:
```bash
git checkout -b branch_name
```

### Merge a branch into the main branch:
```bash
git checkout main
git merge branch_name
```

---

## 7. Undo Changes

### Unstage a file:
```bash
git reset file_name
```

### Revert uncommitted changes to a file:
```bash
git checkout -- file_name
```

### Reset the last commit (keep changes in working directory):
```bash
git reset --soft HEAD~1
```

---

## 8. Viewing History

### View commit history:
```bash
git log
```

### View a simplified commit history:
```bash
git log --oneline
```

---

## 9. Deleting Branches

### Delete a local branch:
```bash
git branch -d branch_name
```

### Delete a remote branch:
```bash
git push origin --delete branch_name
```

---

## 10. Helpful Commands

### Check the current branch:
```bash
git branch
```

### See differences between files:
```bash
git diff
```

### Show commit history with graph:
```bash
git log --oneline --graph
```

---

## Additional Tips

- Use `.gitignore` to ignore files or directories you don’t want to include in your repository.
- Commit often and write clear commit messages.
- Regularly pull changes from the remote repository to keep your local branch updated.

---

For more advanced topics, refer to the [official Git documentation](https://git-scm.com/doc).
