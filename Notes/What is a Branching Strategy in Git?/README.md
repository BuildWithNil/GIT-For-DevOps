# 🌿 Git Branching Strategies

A **branching strategy** is a set of guidelines that a development team uses to manage code changes via branches in a Git repository.

It helps ensure collaboration, maintain code quality, and streamline releases.

---

## 🔧 Why Use a Branching Strategy?

- Keep the `main` branch production-ready
- Allow parallel development (features, bug fixes, experiments)
- Minimize merge conflicts
- Enable CI/CD workflows

---

## 🚀 Common Git Branching Strategies

### 1. Main-Only Strategy

- All work is done directly on the `main` (or `master`) branch
- Suitable for small or solo projects

```
main
```

### 2. Feature Branching

- Create a branch for each feature or task
- Merge into `main` after code review and testing

```
main
 └── feature/login-page
 └── feature/payment-gateway
```

✅ Good for collaboration and clean history

---

### 3. Git Flow

A structured strategy with multiple branches:

- `main`: Production-ready code
- `develop`: Integration branch for features
- `feature/*`: Feature development
- `release/*`: Pre-release preparation
- `hotfix/*`: Emergency fixes on production

```
main ← hotfix
 ↑
release ← develop ← feature
```

✅ Best for large teams and formal release cycles

---

### 4. GitHub Flow

A simplified strategy for modern development:

1. Create a `feature` branch from `main`
2. Commit changes
3. Open Pull Request
4. Review and merge into `main`
5. Deploy

```
main
 └── feature/issue-123
```

✅ Great for continuous delivery and agile workflows

---

### 5. Trunk-Based Development

- All developers commit directly to the `main` branch or very short-lived branches
- Relies on automated testing and CI

✅ Ideal for high-velocity DevOps teams

---

## 🧠 Summary Table

| Strategy            | Best For                     | Branches Used                                  |
|---------------------|------------------------------|------------------------------------------------- |
| Main-Only           | Solo developers              | `main`                                          |
| Feature Branching   | Small/medium teams           | `main`, `feature/*`                             |
| Git Flow            | Large teams, structured dev  | `main`, `develop`, `feature/*`, `release/*`, `hotfix/*` |
| GitHub Flow         | Agile teams, CI/CD           | `main`, `feature/*`                             |
| Trunk-Based         | Fast DevOps workflows        | `main` or short-lived branches                  |

---

## 📝 Tips for Choosing a Strategy

- Small team? Use **Feature Branching** or **GitHub Flow**
- Enterprise project? Consider **Git Flow**
- Moving fast with automation? Try **Trunk-Based Development**
