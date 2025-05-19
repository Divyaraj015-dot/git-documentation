# 📘 Git Commands Cheat Sheet #
 A beginner-friendly guide to commonly used Git commands, complete with descriptions and key concepts. This documentation is structured for easy sharing and 
 professional presentation.

🔧 Git Configuration
git config --global user.name "Your Name"
Sets your Git username globally across all repositories.

git config --global user.email "your-email@example.com"
Sets your Git email globally across all repositories.

🚀 Getting Started
git init
Initializes a new Git repository in the current directory.

git clone <repository-URL>
Clones a remote repository to your local machine.

📋 Staging and Committing Changes
git status
Displays the status of the working directory and staging area.

git add <filename>
Stages a specific file for commit.

git add .
Stages all modified and new files for commit.

git commit -m "Your commit message"
Commits the staged changes with a meaningful message.

🌐 Remote Repositories
git remote add origin <repository-URL>
Connects your local repository to a remote GitHub repository.

git push -u origin main
Pushes your changes to the remote main branch and sets it as the default upstream.

git push
Pushes committed changes to the currently tracked remote branch.

git pull origin main
Pulls the latest changes from the main branch of the remote repository.

🌿 Branching in Git
git branch
Lists all local branches in the repository.

git branch <branch-name>
Creates a new branch.

git checkout <branch-name>
Switches to the specified branch.

git merge <branch-name>
Merges the specified branch into the current branch.

git diff <branch-name>
Shows the difference between the current branch and another.

git branch -d <branch-name>
Deletes the specified local branch.

📚 Git Branching Concepts
🔹 What is a Git Branch?
A Git branch is an isolated workspace that allows you to work on a specific task (like a feature or bug fix) without affecting the main codebase.

🔹 Parent Branch
The branch from which another branch (child) is created.

Typically used as the base for new development.

Often the main or develop branch in most workflows.

🔹 Child Branch
A new branch created from a parent.

Inherits all history from the parent up to the point of creation.

Ideal for working on new features, experiments, or bug fixes.

Can later be merged back into the parent branch.

✅ Best Practices
Always write meaningful commit messages.

Use branches for features, fixes, or experiments.

Regularly pull updates to avoid merge conflicts.

Keep your main branch clean and production-ready.
