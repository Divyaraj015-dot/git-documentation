

1. **git config --global user.name "Your Name"**  
   Sets your Git username globally().

2. **git config --global user.email "your-email@example.com"**  
   Sets your Git email globally for all repositories.

3. **git init**  
   Initializes a new Git repository in the current folder.

4. **git status**  
   Displays the state of the working directory and staging area.

5. **git add "filename"**  
  Stages a specific file for the next commit.

6. **git add .**  
  Stages all modified and new files.

7. **git commit -m "your message"**  
  Commits the staged changes with a message.

8. **git remote add origin repo-URL**  
  Connects your local repository to a remote GitHub repository.

9. **git push -u origin main**  
  Pushes your code to the remote 'main' branch and sets upstream tracking.

10. **git push**  
  Pushes the committed changes to the remote branch.

11. **git clone <repo-URL>**  
  Clones a remote repository to your local machine.

12. **git pull origin main**  
  Pulls the latest changes from the 'main' branch of the remote repository.

13. **git branch**  
  Lists all local branches in the repository.

14. **git branch branch-name**  
  Creates a new branch.

15. **git checkout branch-name**  
  Switches to the specified branch.

16. **git merge branch-name**  
  Merges the specified branch into the current branch.

17. **git diff branch-name**  
    To compare commits,branches,files & more.

19. **git branch -d branch-name**  
  Deletes the specified local branch.
#Branches concepts#
- A Git branch is indeed like a parallel version of your project, allowing you to work on features or experiments without affecting the main codebase.
- Git branches serve as isolated workspaces where you can experiment, develop new features, or fix bugs without impacting the main codebase.
- This isolation allows for safer development practices and more organized workflows.
# Parent Branch
- A parent branch in Git refers to the branch from which another branch is created.
- It serves as the starting point or base for the new branch.
- The parent branch is typically the branch you are currently on when creating a new branch.
- In many workflows, the parent branch is considered the "base" branch.
- Understanding the parent branch helps in managing merges and resolving conflicts.
# Child Branch #
- A child branch in Git is a branch that is created from another branch (the parent branch). 
- It represents a diverging line of development.
- The child branch inherits the commit history of the parent branch up to the point of creation.
- Developing in a child branch allows for isolated work without affecting the parent branch.
- Eventually, changes from the child branch can be merged back into the parent branch.



