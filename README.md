# github-learning.

This repository is dedicated to helping new contributors learn the fundamental concepts and commands of **Git** and the collaboration workflow on **GitHub**.

---

## 💻 Essential Git Commands for Your Workflow

The following table provides detailed descriptions and use cases for the Git commands you will use most often:

| Command | Description & Use Case | Example |
| :--- | :--- | :--- |
| `git init` | **Initializes** a new, empty Git repository in the current directory. This command creates the hidden `.git` folder, which tracks all changes. | `git init` |
| `git clone [url]` | **Downloads** an existing remote repository (like one on GitHub) to your local machine, creating a local copy you can work on. | `git clone https://github.com/user/repo.git` |
| `git status` | **Shows** the current state of the working directory and the staging area. It lets you see which changes have been staged, which haven't, and which files are untracked. | `git status` |
| `git add [file]` | **Adds** changes from the working directory to the staging area. The staging area is where you prepare a snapshot before committing. Use `.` to add all changes. | `git add README.md` or `git add .` |
| `git commit -m "[message]"` | **Records** the staged snapshot to the repository history. The message should clearly and concisely describe the changes you made. | `git commit -m "feat: add documentation for essential git commands"` |
| `git branch [name]` | **Creates** a new branch. Branches are crucial for developing features or fixes in isolation without affecting the main codebase. | `git branch feat/new-login-ui` |
| `git checkout [name]` | **Switches** from one branch to another. This updates your working directory to match the content of the target branch. Use `git checkout -b [new_branch]` to create and switch in one step. | `git checkout main` |
| `git merge [branch]` | **Integrates** changes from the specified branch into your current branch. This is often used to bring a completed feature branch into the `main` or `dev` branch. | `git merge feat/new-login-ui` |
| `git push` | **Uploads** your local branch commits to the remote repository (e.g., GitHub). This makes your changes available for others and for opening a Pull Request. | `git push origin my-feature-branch` |
| `git pull` | **Fetches** and **downloads** content from the remote repository and immediately updates your local working branch to match the remote's changes. | `git pull origin main` |

---

## 💡 Advanced & Utility Commands

These commands are useful for inspecting history and fixing mistakes.

| Command | Description & Use Case | Example |
| :--- | :--- | :--- |
| `git log` | **Displays** the commit history for the current branch, showing who made what changes and when. The `--oneline` option provides a concise view. | `git log --oneline` |
| `git diff` | **Shows** the differences between various states of the repository (e.g., between the working directory and the staging area, or between two commits). | `git diff` |
| `git reset [file]` | **Unstages** a file (removes it from the staging area) without discarding the changes you made to the file in your working directory. Use with caution! | `git reset index.html` |
| `git revert [commit]` | **Creates a new commit** that undoes the changes introduced in a prior commit. This is the safest way to undo history that has already been pushed to the remote. | `git revert HEAD` |
| `git remote -v` | **Lists** the shortnames and URLs for your remote repositories. | `git remote -v` |

---

## 🚀 Recommended Contribution Workflow

1.  **Clone** the repo: `git clone [repository-url]`
2.  **Create** and switch to a new branch: `git checkout -b your-branch-name`
3.  **Make** your changes to the files.
4.  **Stage** the changes: `git add .`
5.  **Commit** the changes with a clear message: `git commit -m "feat: descriptive commit message"`
6.  **Push** your branch: `git push origin your-branch-name`
7.  **Open a Pull Request** (PR) on GitHub from your new branch to the main branch.

*For PR submission guidelines, please check the [PULL\_REQUEST\_TEMPLATE.md](.github/PULL_REQUEST_TEMPLATE.md) file.*