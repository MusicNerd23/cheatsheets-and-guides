# Git & GitHub Cheat Sheet 🚀

## 📌 1. Initialize a Repository
```bash
git init
```
- Creates a new Git repository in the current directory.

## 📌 2. Create a `.gitignore` File
Before adding files, create a `.gitignore` file to exclude unnecessary files.

### Recommended `.gitignore` for Python Projects:
```
# Virtual environment
venv/

# Byte-compiled / cached files
__pycache__/
*.py[cod]
*$py.class

# Distribution / Packaging
*.egg-info/
dist/
build/

# Logs and Databases
*.log
*.sqlite3

# VS Code & IDE Specific
.vscode/
.idea/
*.sublime-workspace

# Jupyter Notebook Checkpoints
.ipynb_checkpoints/

# OS-Specific
.DS_Store
Thumbs.db
```

## 📌 3. Add Files to Git
```bash
git add .
```
- Stages all files for commit.

## 📌 4. Commit Changes
```bash
git commit -m "Initial commit"
```
- Saves changes with a meaningful commit message.

## 📌 5. Connect to a Remote Repository
```bash
git remote add origin <repository_url>
```
- Links your local repo to GitHub.

## 📌 6. Push Changes to GitHub
```bash
git push -u origin main
```
- Uploads changes to GitHub.

## 📌 7. Check Repository Status
```bash
git status
```
- Shows the current state of your working directory.

## 📌 8. View Commit History
```bash
git log --oneline --graph --decorate --all
```
- Displays a concise commit history.

## 📌 9. Pull Updates from Remote
```bash
git pull origin main
```
- Fetches and merges the latest updates from GitHub.

## 📌 10. Create and Switch Branches
```bash
git checkout -b feature-branch
```
- Creates a new branch and switches to it.

```bash
git checkout main
```
- Switches back to the `main` branch.

## 📌 11. Merge a Branch
```bash
git checkout main
git merge feature-branch
```
- Merges `feature-branch` into `main`.

## 📌 12. Resolve Merge Conflicts
If there’s a conflict:
1. Open conflicting files and manually fix issues.
2. Stage the resolved files:
   ```bash
   git add .
   ```
3. Commit the merge:
   ```bash
   git commit -m "Resolved merge conflict"
   ```

## 📌 13. Undo Changes
- Unstage a file:
  ```bash
  git reset HEAD <file>
  ```
- Discard local changes:
  ```bash
  git checkout -- <file>
  ```

## 📌 14. Delete a Branch
- Delete a local branch:
  ```bash
  git branch -d feature-branch
  ```
- Delete a remote branch:
  ```bash
  git push origin --delete feature-branch
  ```

## 📌 15. Revert to a Previous Commit
```bash
git reset --hard <commit_id>
```
- Moves the branch to a previous commit and discards all changes.

---

### **✅ How to Use This**
1. **Save this as `github_cheat_sheet.md`** in your `cheatsheets-and-guides` repo.
2. **Commit and push** it to GitHub.
3. **Access it anytime** from GitHub or your local machine.

🚀 Now you have a **GitHub cheat sheet ready to go** in your repository! Let me know if you need any adjustments.
