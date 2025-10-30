# Github-Commands
This readme file give you insights of essential github commands

# 🧩 Essential Git Commands Guide

A complete guide to essential Git commands for Xcode, Swift, or any development workflow.  
Copy and paste commands directly from here — works perfectly in Terminal or VS Code.

---

## 🏁 Initialize & Setup
```bash
# Initialize git in your project
git init

# Configure your name and email
git config --global user.name "Your Name"
git config --global user.email "your-email@example.com"

# Check current configuration
git config --list
```

---

## 📂 Repository Setup
```bash
# Clone an existing repository
git clone https://github.com/username/repository.git

# Add remote repository (link your local repo to GitHub)
git remote add origin https://github.com/username/repository.git

# Verify remote link
git remote -v
```

---

## 📦 Basic Workflow
```bash
# Check the current status
git status

# Add all new or modified files
git add .

# Add a specific file
git add filename.swift

# Commit your changes with a message
git commit -m "Initial commit"
```

---

## 🌐 Push & Pull
```bash
# Rename branch to main (if needed)
git branch -M main

# Push code to GitHub
git push -u origin main

# Push further commits
git push

# Pull latest changes from GitHub
git pull
```

---

## 🌳 Branching
```bash
# Create a new branch
git branch feature-branch

# Switch to a branch
git checkout feature-branch

# Create & switch in one command
git checkout -b new-branch

# Merge another branch into current
git merge feature-branch

# Delete a branch
git branch -d feature-branch
```

---

## 🧹 Undo & Clean
```bash
# Undo last commit (keep changes staged)
git reset --soft HEAD~1

# Undo last commit (remove changes)
git reset --hard HEAD~1

# Remove a file from staging
git reset filename.swift

# Discard all local changes
git checkout -- .
```

---

## 🕵️ Inspecting Changes
```bash
# View commit history
git log

# View a concise log
git log --oneline --graph --decorate --all

# Compare changes
git diff
```

---

## ⚙️ Tagging & Releases
```bash
# Create a tag
git tag v1.0

# Push tags
git push --tags

# Delete a tag
git tag -d v1.0
```

---

## 🔐 Authentication (GitHub Token Setup)
```bash
# Store credentials to avoid re-entering
git config --global credential.helper store

# After successful login, credentials are saved in ~/.git-credentials
```

---

## 🧠 Miscellaneous
```bash
# Check remote branches
git branch -r

# Delete remote branch
git push origin --delete branch-name

# Stash changes temporarily
git stash
git stash pop

# Show current branch
git branch --show-current
```

---

## ✅ Common Workflow Summary
```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/username/repo.git
git push -u origin main
```

---

### 💡 Tip
To permanently store your GitHub credentials (token):
```bash
git config --global credential.helper store
```

Now your credentials will be remembered for future pushes.

---
