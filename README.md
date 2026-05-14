Practice Repository

Welcome! 👋
This repository is created for practicing Git and GitHub.

I’m using this space to learn and revise:

Git commands (commit, push, pull, branching, merging)

GitHub workflows

Pull requests & collaboration

Managing repositories and version control basics

Feel free to ignore the contents — this repo is mainly for my learning and experimentation or you can use it if this helps...
I’ll keep updating it as I improve. 🚀
Thankyou


UPDATE :=

# 🚀 Git & GitHub Developer Cheat Sheet

> Simple • Clean • Real Developer Workflow • Copy-Paste Ready

---

# 📁 PROJECT SETUP

```bash
# Create project folder
mkdir myproject

# Enter folder
cd myproject

# Initialize Git
git init
```

---

# 📄 CREATE FILES & FOLDERS

```bash
# Create folders
mkdir backend frontend venv

# Create files
touch backend/app.py
touch frontend/style.css
touch secret.txt
```

---

# 🚫 .GITIGNORE (IGNORE FILES)

```bash
# Create .gitignore
touch .gitignore

# Ignore virtual environment
echo "venv/" >> .gitignore

# Ignore secret file
echo "secret.txt" >> .gitignore
```

---

# 🔍 CHECK PROJECT STATUS

```bash
git status
```

---

# ➕ STAGE FILES

```bash
# Add everything
git add .

# Add specific folder
git add backend/

# Add specific file
git add backend/app.py
```

---

# ↩️ UNSTAGE FILES

```bash
# Remove everything from staging
git restore --staged .

# Remove folder from staging
git restore --staged backend/

# Remove file from staging
git restore --staged file.txt
```

---

# 🧯 FIX STAGING ISSUE (Before First Commit)

```bash
git rm --cached -r .
```

---

# 💾 COMMIT CHANGES

```bash
git commit -m "your message"
```

---

# 🔗 CONNECT TO GITHUB

```bash
# Connect local repo to GitHub repo
git remote add origin https://github.com/USERNAME/REPO.git

# Rename branch to main
git branch -M main
```

---

# 🚀 PUSH TO GITHUB

```bash
# First push
git push -u origin main
```

### ⚠️ If GitHub Already Has Files

```bash
git pull origin main --allow-unrelated-histories

git push -u origin main
```

### ⚠️ Force Push (Danger)

```bash
git push -u origin main --force
```

---

# 📥 CLONE EXISTING REPOSITORY

```bash
git clone https://github.com/USERNAME/REPO.git

cd REPO
```

---

# 🔄 UPDATE LOCAL REPOSITORY

```bash
git pull
```

---

# 🗂️ DELETE FILES / FOLDERS

```bash
# Delete file
rm file.txt

# Delete folder
rm -r foldername
```

---

# 📌 NAVIGATION COMMANDS

```bash
# Enter folder
cd foldername

# Go back
cd ..

# Show files
ls

# Show hidden files
ls -a
```

---

# 📜 COMMIT HISTORY

```bash
git log
```

---

# 🌿 BRANCHING WORKFLOW

## 🌱 Create New Branch

```bash
git checkout -b feature-name
```

### OR (Modern Way)

```bash
git switch -c feature-name
```

---

## 📋 View Branches

```bash
# Local branches
git branch

# Local + remote branches
git branch -a
```

---

## ✍️ Work & Commit

```bash
git add .

git commit -m "implemented feature"
```

---

## 🚀 Push Feature Branch

```bash
git push -u origin feature-name
```

---

# 🔁 UPDATE FEATURE BRANCH WITH MAIN

```bash
# Switch to main
git checkout main

# Get latest updates
git pull origin main

# Return to feature branch
git checkout feature-name

# Merge main into branch
git merge main
```

---

# 🔀 MERGE FEATURE → MAIN

```bash
# Switch to main
git checkout main

# Merge feature branch
git merge feature-name

# Push updated main
git push origin main
```

---

# 🌐 PULL REQUEST (REAL COMPANY FLOW)

## 1️⃣ Push Branch

```bash
git push origin feature-name
```

## 2️⃣ Open GitHub

- Go to repository
- Click **Compare & Pull Request**

## 3️⃣ Create PR

- Add title
- Add description
- Click **Create Pull Request**

## 4️⃣ Code Review

- Team reviews code
- Fix requested changes if needed

## 5️⃣ Merge PR

- Click **Merge Pull Request**

---

# 🧹 CLEANUP AFTER MERGE

```bash
# Delete local branch
git branch -d feature-name

# Delete remote branch
git push origin --delete feature-name
```

---

# ⚠️ MERGE CONFLICT FIX

```bash
# Check conflicts
git status
```

Then manually fix:

```txt
<<<<<<< HEAD
your code
=======
incoming code
>>>>>>> branch
```

After fixing:

```bash
git add .

git commit -m "fixed merge conflict"
```

---

# 🔄 FETCH VS PULL

```bash
# Download updates only
git fetch

# Download + merge updates
git pull origin main
```

---

# 🧠 REAL INDUSTRY WORKFLOW

```bash
# 1. Create branch
git checkout -b feature-name

# 2. Work on feature
git add .

git commit -m "work done"

# 3. Push branch
git push origin feature-name
```

### Then on GitHub:
- Open Pull Request
- Code Review
- Merge PR
- Delete Branch

---

# ✅ MOST IMPORTANT COMMANDS

```bash
git status

git add .

git commit -m "message"

git push

git pull
```

---

# 🎯 QUICK UNDERSTANDING

| Command | Purpose |
|---|---|
| `git init` | Start Git repo |
| `git status` | Check changes |
| `git add .` | Stage files |
| `git commit` | Save snapshot |
| `git push` | Upload to GitHub |
| `git pull` | Get latest changes |
| `git branch` | View branches |
| `git checkout -b` | Create branch |
| `git merge` | Combine branches |

---

# 🚀 DONE

You now know:
- Git basics
- GitHub workflow
- Branching
- Pull Requests
- Merge conflicts
- Real developer workflow
