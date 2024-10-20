# Command Reference Guide

## 1. File System Management

### Creating Directories
mkdir git for devops
mkdir file2

### Listing Files
ls
ls -al

### Navigating Directories
cd git
cd mkdir for devops
pwd

### Creating Files
touch nibba.txt nibbi.txt
touch file1
touch pwd.txt

---

## 2. Git Basics

### Initializing a Repository
git init

### Checking Status
git status

### Adding Files to Staging
git add nibbi.txt
git add nibba.txt
git add pwd.txt
git add file1
git add file2
git add .

### Removing Files from Staging
git rm --cached nibba.txt

### Committing Changes
git commit -m "add nibba and nibbi"
git commit -m "adding new file"
git commit -m "another file"

---

## 3. Branch Management

### Creating and Switching Branches
git branch
git branch -b dev
git checkout -b dev
git checkout master
git checkout dev

### Viewing Branches
git branch

---

## 4. Git Logs and History

### Viewing Commit History
git log
git log --oneline
git logs

### Resetting Commits
git reset
git reset --soft 1a03e18

---

## 5. Git Configuration

### Setting Global Configurations
git config --global user.email "kapilrajc05@gmail.com"
git config --global user.name "kapilraj.vidafoneidea"

---

## 6. Exiting and History

### Exiting Terminal
exit

### Viewing Command History
history
