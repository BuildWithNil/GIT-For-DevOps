
# 📘 Git Commands Cheat Sheet

Git is a distributed version control system widely used in DevOps and software development. This guide includes essential Git commands with examples.

---

## 🔧 Configuration

```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
git config --list         # View all config settings
```

---

## 📁 Repository Setup

```bash
git init                  # Initialize a new Git repository
git clone <repo_url>      # Clone an existing repo
```

---

## 📄 Basic Snapshotting

```bash
git status                # Check the status of working directory and staging area
git add <file>            # Add file to staging area
git add .                 # Add all changes to staging
git commit -m "Message"   # Commit staged changes
```

---

## 🔄 Branching & Merging

```bash
git branch                # List all branches
git branch <name>         # Create a new branch
git checkout <name>       # Switch to a branch
git checkout -b <name>    # Create and switch to a new branch
git merge <branch>        # Merge a branch into the current one
```

---

## 🔁 Remote Repositories

```bash
git remote -v                                # View remote URLs
git remote add origin <repo_url>             # Add a remote repo
git push -u origin main                      # Push local 'main' branch to remote
git push                                     # Push changes
git pull                                     # Pull changes from remote
git fetch                                    # Fetch latest changes
```

---

## 🕓 Commit History

```bash
git log                                      # View commit history
git log --oneline                            # One-line commit summary
```

---

## 🛠 Undoing Changes

```bash
git restore <file>                           # Discard changes in working directory
git reset <file>                             # Unstage a file
git reset --hard                             # Discard all changes and reset to last commit
```

---

## 🔍 Stashing

```bash
git stash                                    # Stash current changes
git stash list                               # List stashes
git stash apply                              # Re-apply the last stash
```

---

## ❌ Remove Remote Link

```bash
git remote remove origin                     # Remove remote URL
```

---

## 📤 GitHub First Push (New Repo)

```bash
echo "# MyProject" >> README.md
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/username/repo.git
git push -u origin main
```

---

## 📌 Git Tags

```bash
git tag v1.0                                 # Create tag
git tag                                      # List tags
git push origin v1.0                         # Push specific tag
```

---

## 🧹 Clean Up

```bash
git clean -n                                 # Show files to be removed
git clean -f                                 # Force remove untracked files
```

---

## 📚 Helpful Tips

- `.gitignore`: List files/folders to be ignored by Git.
- Always commit small, meaningful changes.
- Use branches for feature development.
- Keep `main` or `master` branch stable.

---

