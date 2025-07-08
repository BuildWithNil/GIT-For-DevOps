# Git Three-Stage Architecture

Git has a three-stage architecture, consisting of the **Working Directory**, the **Staging Area**, and the **Repository**.

---

## 🗂️ Working Directory

The **working directory** is the directory on your local machine where all files and changes are stored.

1. It acts as a workspace for modifications and updates before they are committed.
2. Users can create new files or modify existing ones independently.
3. Enables experimentation with different versions or branches without affecting the main repository.

---

## 📥 Staging Area

The **staging area** is where developers select which changes to include in the next commit.

- It acts as an intermediate step between the working directory and the repository.
- Only the files added with `git add` go to the staging area.
- You can commit directly with `git commit -am "message"`, but it still stages files implicitly.

---

## 🗃️ Repository (Git Directory)

The **repository** is the final level where the project's full history is stored.

- When changes are committed, Git takes a snapshot of the staging area.
- Stores all codebase versions (current and previous).
- Ensures robust version control and recovery.

---

# Git Core Concepts

## 🔁 Repository

A **repository** is where all project data and revision history are stored. It can be **local** or **remote**.

- Contains branches, commits, and tags.

## ✅ Commit

A **commit** is a snapshot of changes in the project.

- Use `git add` to stage changes, then `git commit` to save them.
- Each commit has a unique hash and descriptive message.

## 🔖 Tags

**Tags** are static references to commits.

- Used to mark important points (e.g., releases).
- Unlike branches, tags do not change.

## 🖼️ Snapshots

Git saves data as **snapshots** of the project rather than diffs.

- Each commit is a complete snapshot of the project.
- Enables fast branching and merging.

## 🔁 Push-Pull Mechanism

Git uses a **push-pull model** in collaborative workflows.

### Push

Uploads local commits to a remote repository.

```bash
git push origin main
```

### Pull

Fetches and integrates changes from a remote repository.

```bash
git pull origin main
```

## 🌿 Branching Strategy

Branching allows independent development paths.

### Common Strategies:

- **Feature Branching**: New branch per feature.
- **Gitflow Workflow**: Structured with master, develop, feature, release, and hotfix branches.
- **GitHub Flow**: Simplified, single main branch with frequent deployments.

---

> Git’s three-stage design helps developers track, test, and commit changes effectively for collaborative software development.
