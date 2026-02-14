 Git Version Control Notes

## What is Git?
Git is a distributed version control system used to track changes in code and collaborate with others.

---

# Git Configuration Commands

```bash
git config --global --add safe.directory <folder_path>
```
→ Mark a directory as safe.

```bash
git --version
```
→ Show installed Git version.

---

# Initialize & Remote Setup

```bash
git init
```
→ Initialize a new Git repository.

```bash
git remote add origin <repository_link>
```
→ Connect local project with remote repository.

```bash
git remote -v
```
→ Show connected remote URLs.

```bash
git branch -M main
```
→ Rename current branch to main.

```bash
git push origin main
```
→ Push code to remote main branch.

---

# Basic Git Commands

```bash
ls -a
```
→ Show hidden files (including .git folder).

```bash
git clone <repo_link>
```
→ Clone a repository.

```bash
git status
```
→ Check current repository status.

```bash
git add <file_name>
```
→ Stage a specific file.

```bash
git add .
```
→ Stage all changed files.

```bash
git commit -m "Your message"
```
→ Commit staged changes.

```bash
git push origin main
```
→ Upload changes to GitHub.

---

# Pull Updates

```bash
git pull origin main
```
→ Pull latest changes from remote.

```bash
git pull origin main --allow-unrelated-histories
```
→ Merge unrelated histories.

```bash
git pull origin main --allow-unrelated-histories --no-rebase
```
→ Pull without rebasing.

---

# Git File States

- **Untracked** → Git is not tracking the file.
- **Modified** → File changed but not staged.
- **Staged** → Ready to commit.
- **Unmodified** → No changes detected.

---

# Git Workflow

```
Working Directory → Staging Area → Local Repository → Remote Repository
```

Step-by-step:
1. Modify file
2. `git add`
3. `git commit`
4. `git push`

---

# Git Branch

```bash
git branch
```
→ Show all branches.

```bash
git checkout <branch_name>
```
→ Switch branch.

```bash
git checkout -b <new_branch_name>
```
→ Create and switch to new branch.

```bash
git branch -d <branch_name>
```
→ Delete a branch.

---

# Merge Code

### Way 1 (Local Merge)

```bash
git diff
git merge <branch_name>
```

### Way 2 (GitHub)
→ Create a Pull Request (PR).

---

# ⚠️ Resolve Merge Conflict

1. Open conflicted file
2. Fix conflict manually
3. `git add .`
4. `git commit`

---

# Git Undoing

```bash
git restore <file_name>
```
→ Discard changes in working directory.

```bash
git reset HEAD <file_name>
```
→ Unstage a file.

```bash
git reset --hard
```
→ Remove all changes (Dangerous ⚠️)

```bash
git stash
```
→ Save changes temporarily.

```bash
git stash pop
```
→ Reapply stashed changes.

---

# Pro Tip

Always check status before pushing:
```bash
git status
```

---

# Remember

> Git never deletes your work silently.  
> It protects your changes until you decide what to do. 🚀 Git Version Control Notes

##  What is Git?
Git is a distributed version control system used to track changes in code and collaborate with others.

---

# Git Configuration Commands

```bash
git config --global --add safe.directory <folder_path>
```
→ Mark a directory as safe.

```bash
git --version
```
→ Show installed Git version.

---

# Initialize & Remote Setup

```bash
git init
```
→ Initialize a new Git repository.

```bash
git remote add origin <repository_link>
```
→ Connect local project with remote repository.

```bash
git remote -v
```
→ Show connected remote URLs.

```bash
git branch -M main
```
→ Rename current branch to main.

```bash
git push origin main
```
→ Push code to remote main branch.

---

# Basic Git Commands

```bash
ls -a
```
→ Show hidden files (including .git folder).

```bash
git clone <repo_link>
```
→ Clone a repository.

```bash
git status
```
→ Check current repository status.

```bash
git add <file_name>
```
→ Stage a specific file.

```bash
git add .
```
→ Stage all changed files.

```bash
git commit -m "Your message"
```
→ Commit staged changes.

```bash
git push origin main
```
→ Upload changes to GitHub.

---

#  Pull Updates

```bash
git pull origin main
```
→ Pull latest changes from remote.

```bash
git pull origin main --allow-unrelated-histories
```
→ Merge unrelated histories.

```bash
git pull origin main --allow-unrelated-histories --no-rebase
```
→ Pull without rebasing.

---

# 📌 Git File States

- **Untracked** → Git is not tracking the file.
- **Modified** → File changed but not staged.
- **Staged** → Ready to commit.
- **Unmodified** → No changes detected.

---

# Git Workflow

```
Working Directory → Staging Area → Local Repository → Remote Repository
```

Step-by-step:
1. Modify file
2. `git add`
3. `git commit`
4. `git push`

---

# Git Branch

```bash
git branch
```
→ Show all branches.

```bash
git checkout <branch_name>
```
→ Switch branch.

```bash
git checkout -b <new_branch_name>
```
→ Create and switch to new branch.

```bash
git branch -d <branch_name>
```
→ Delete a branch.

---

# Merge Code

### Way 1 (Local Merge)

```bash
git diff
git merge <branch_name>
```

### Way 2 (GitHub)
→ Create a Pull Request (PR).

---

#  Resolve Merge Conflict

1. Open conflicted file
2. Fix conflict manually
3. `git add .`
4. `git commit`

---

#  Git Undoing

```bash
git restore <file_name>
```
→ Discard changes in working directory.

```bash
git reset HEAD <file_name>
```
→ Unstage a file.

```bash
git reset --hard
```
→ Remove all changes (Dangerous ⚠️)

```bash
git stash
```
→ Save changes temporarily.

```bash
git stash pop
```
→ Reapply stashed changes.

---

#  Pro Tip

Always check status before pushing:
```bash
git status
```

---

# Remember

> Git never deletes your work silently.  
> It protects your changes until you decide what to do.