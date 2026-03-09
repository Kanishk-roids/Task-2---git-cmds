# Git Commands Reference

This repository contains commonly used Git commands with simple explanations.

---

## 1. Check Git Version

```bash
git --version
```

Shows the version of Git installed on your system.

---

## 2. Configure Git (Username and Email)

```bash
git config --global user.email "your-email@example.com"
git config --global user.name "Your Name"
git config --list
```

Sets your username and email for Git commits.
`git config --list` displays all current configuration settings.

---

## 3. Creating a Repository

```bash
git status
git init
```

`git status` shows the current state of your repository.
`git init` initializes a new Git repository and creates the hidden `.git` folder.

---

## 4. Staging Files

```bash
git add <file>
git add <file1> <file2>
git status
```

Stages specific files so they can be included in the next commit.

---

## 5. Commit Changes

```bash
git commit -m "commit message"
git status
```

Saves the staged changes to the repository with a message.

---

## 6. View Commit History

```bash
git log
git log --oneline
```

Displays the history of commits made in the repository.

---

## 7. Change Default Editor

```bash
git config --global core.editor "code --wait"
```

Changes the default Git editor to Visual Studio Code.

---

## 8. Add Remote Repository

```bash
git remote add origin <repository-url>
git remote -v
```

Connects your local repository to a remote repository.

---

## 9. Push Code to Remote Repository

```bash
git push origin main
git push -u origin main
```

Uploads local commits to the remote repository.

---

## 10. Fetch Changes

```bash
git fetch <remote-name>
```

Downloads changes from the remote repository but does not merge them.

---

## 11. Pull Changes

```bash
git pull origin main
```

Fetches and merges changes from the remote repository.

---

## 12. List Branches

```bash
git branch
```

Displays all branches in the repository.

---

## 13. Create and Switch Branch

```bash
git branch new-branch
git switch new-branch
git switch -c another-branch
```

Creates a new branch and allows switching between branches.

---

## 14. Rename a Branch

```bash
git branch -m <old-branch-name> <new-branch-name>
```

Renames an existing branch.

---

## 15. Delete a Branch

```bash
git branch -d <branch-name>
```

Deletes a branch that is no longer needed.

---

## 16. Compare Changes

```bash
git diff
```

Shows the difference between file versions.

---

## 17. Stash Changes

```bash
git stash
git stash save "work in progress"
git stash list
git stash clear
```

Temporarily stores changes so you can work on something else.

---

## 18. Create and Manage Tags

```bash
git tag <tag-name>
git tag -a <tag-name> -m "release version"
git tag
git tag -d <tag-name>
git push origin <tag-name>
```

Tags are used to mark important commits such as release versions.

---

## 19. Rebase

```bash
git checkout feature-branch
git rebase main
git add <resolved-files>
git rebase --continue
```

Reapplies commits from one branch onto another to keep the history cleaner.

---

## 20. Git Reflog and Reset

```bash
git reflog
git reset --hard <commit-hash>
git reset --hard HEAD@{1}
```

`git reflog` shows a record of all actions in the repository and can help recover lost commits.
