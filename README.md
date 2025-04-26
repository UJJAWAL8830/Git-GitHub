# Git-GitHub
All my learnings of git and github can be access through this repository.

# Git and GitHub Commands Cheat Sheet 📚

---

## 1. Git Basic Commands

| Command | Description |
|:---|:---|
| `git init` | Initialize a new Git repository in a local folder. |
| `git status` | Check the status of files (untracked, modified, staged) in the repository. |
| `git add <file_name>` | Stage a specific file for commit. |
| `git add .` | Stage **all** changes (new, modified files). |
| `git commit -m "Message"` | Commit staged changes with a meaningful message. |
| `git commit -am "Message"` | Add and commit in one step (only for modified files, not new ones). |
| `git log` | View the commit history. |

---

## 2. Git Configuration Commands

| Command | Description |
|:---|:---|
| `git config --global user.name "Your Name"` | Set your Git username globally. |
| `git config --global user.email "youremail@example.com"` | Set your Git email globally. |
| `git config --list` | View all global configurations (username, email, editor, etc.). |

---

## 3. Clone an Existing Repository

```bash
git clone <github-repository-link>
```
- Example: Copy the HTTPS link from GitHub and clone it into your system.

---

## 4. Remote Repository Commands

| Command | Description |
|:---|:---|
| `git remote add origin <repo-https-link>` | Connect your local repo to a remote GitHub repository. |
| `git push origin main` | Push local commits to GitHub on the `main` branch. |
| `git push -u origin main` | Push and set upstream; next pushes can be done just by `git push`. |
| `git pull origin main` | Pull (fetch and merge) latest changes from GitHub to your local repo. |

> ⚡ **Note:**  
> - `git push` = local → GitHub (Upload)  
> - `git pull` = GitHub → local (Download)

---

## 5. Branch Management Commands

| Command | Description |
|:---|:---|
| `git branch` | List all local branches. |
| `git branch -M main` | Rename the current branch to `main`. |
| `git checkout <branch_name>` | Switch to a different branch. |
| `git checkout -b <new_branch_name>` | Create and switch to a new branch. |
| `git branch -d <branch_name>` | Delete a local branch. |
| `git push origin <branch_name>` | Push the branch to GitHub after creating locally. |

---

## 6. Merging Branches

| Command | Description |
|:---|:---|
| `git diff <branch_name>` | Compare differences between current branch and another branch. |
| `git merge <branch_name>` | Merge changes from the specified branch into the current branch. |
| **Alternative:** Create a **Pull Request (PR)** on GitHub to merge branches visually.

---

## 7. Summary Diagram ✨

```plaintext
Local Repo (your computer)
    ⬇️ push
Remote Repo (GitHub server)
    ⬆️ pull
```
- **Push** = Upload your changes
- **Pull** = Download latest updates

---

## Notes 📝

- After creating a new branch locally, **always push** it to GitHub using:
  ```bash
  git push origin <branch_name>
  ```
- After deleting a branch locally, if you want to **delete it from GitHub**, use:
  ```bash
  git push origin --delete <branch_name>
  ```

---

