

#  📗 Git Commands Cheat Sheet #
A beginner-friendly guide to commonly used Git commands, complete with descriptions and key concepts. This documentation is structured for easy sharing and professional presentation.
## 🔧 Git Configuration ##
 **git config --global user.name "Your Name"**  
 
    Sets your Git username globally().

 **git config --global user.email "your-email@example.com"**  
 
    Sets your Git email globally for all repositories.

## 🛠️ Repository Setup ##
 **git init**  
 
    Initializes a new Git repository in the current folder.
 **git clone <repository-url>**  
 
    Clones a remote repository to your local machine.
 **git remote add origin <repository-url>**  
 
    Connects your local repository to a remote GitHub repository.




## 📄 Staging and Committing ##
 **git status**  
 
    Displays the state of the working directory and staging area.
 **git add <filename>**  
 
    Stages a specific file for the next commit.
 **git add .**  
 
    Stages all modified and new files.  
  **git commit -m "your message"**  
  
     Commits the staged changes with a message.

## ⬆️ Pushing and Pulling ##
  **git push -u origin main**  
  
    Pushes your code to the remote main branch and sets upstream tracking.
  **git push**  
  
    Pushes the committed changes to the remote branch.
  **git pull origin main**  
  
    Pulls the latest changes from the main branch of the remote repository.

## 🌿Branch Management ##
 **git branch**  
 
    Lists all local branches in the repository.

 **git branch <branch-name>**  
 
    Creates a new branch.

 **git checkout <branch-name>**  
 
    Switches to the specified branch.
 **git merge <branch-name>**  
 
    Merges the specified branch into the current branch.
 **git diff <branch-name>**  
 
    Compares differences between branches, commits, or files.
 **git branch -d <branch-name>**  
 
    Deletes the specified local branch.


## 🌱 Git Branching Concepts ##
🔹 What is a Branch?
     A Git branch is a parallel version of your project. It allows you to develop features, fix bugs, or experiment without affecting the main codebase. Branches 
     provide a safe and organized workflow for both individuals and teams.

🔹 Parent Branch:
   A parent branch is the original branch from which a new branch is created.
   * It acts as the base or starting point.
   * Typically, the main or develop branch serves as the parent.
   * Understanding parent branches helps prevent conflicts and improves  collaboration.

🔹 Child Branch:
   A child branch is derived from another branch (the parent).
   * It contains all commit history from the parent up to the point of creation. 
   * Useful for isolated development of new features or fixes.
   * Changes from the child branch can be merged back into the parent branch when ready.

