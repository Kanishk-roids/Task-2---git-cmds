# Task-2---git-cmds

1. Check Git Version
   git --version

2. Configure Git (Username & Email)
   git config --global user.email "[email protected]"
   git config --global user.name "Your Name"
   git config --list

   git config sets your Git username and email which will be attached to commits.
   git config --list shows all configuration settings currently applied.

3. Creating a Repository
   git status
   git init

   git status shows the current state of your repository.
   git init creates a new Git repository and adds a hidden .git folder to track changes.


4. Staging Files
   Stage is a way to tell Git to track specific files.

   git init
   git add <file> <file2>
   git status

   git add adds files to the staging area so they are ready to be committed.

5. Commit Changes
   git commit -m "commit message"
   git status

   git commit saves the staged changes permanently as a snapshot of your project.

6. View Commit History
   git log
   git log --oneline

   git log shows the full commit history of the repository.
   git log --oneline shows a shorter, compact version.

7. Add Remote Repository
   git remote add origin <remote-url>
   git remote -v

   git remote add origin links your local repository to a remote repository (like GitHub).
   git remote -v shows the remote URLs connected to your repository.

8. Push Code to GitHub
   git push origin main
   git push -u origin main

   git push origin main uploads your commits to the remote repository.
   -u sets the upstream branch so future pushes don’t need the remote name.

9. Fetch Code
