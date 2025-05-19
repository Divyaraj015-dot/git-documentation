

#  📗 Git Commands for Beginners #
A beginner-friendly guide to commonly used Git commands, complete with descriptions and key concepts. This documentation is structured for easy sharing and professional presentation.
## 🔧 Git Configuration ##
```bash
git config --global user.name "Your Name"
```


Set your global Git username.
```bash
    git config --global user.email "your-email@example.com"
``` 
 
   Set your global Git email

## 🛠️ Repository Setup ##
```bash
git init
```
 Create a new Git repository locally.
 ```bash
git clone <repository-url>
```
 
   Copy a remote repository to your machine.

   
```bash
git remote add origin <repository-url>
``` 
 
  Link your local repo to a remote one.




## 📄 Staging and Committing ##
```bash
git status
``` 
 
Show changes and staged files 
   
```bash
    git add <filename>
``` 
 Stage one file for commit.
 ```bash
git add .
```
 
 
Stage all changed files.  
```bash
 git commit -m "your message"
```  
  Save staged changes with a message.

## ⬆️ Pushing and Pulling ##
```bash
git push -u origin main
```
  
  Push to remote main branch and track it.  
   
```bash
git push
```  
  
 Push committed changes to remote.
```
git pull origin main
``` 
  
  Fetch and merge changes from remote..

## 🌿Branch Management ##
```bash
git branch
``` 
 
 List local branches.
```bash
    git branch <branch-name>
```
 
  Create a new branch.

```bash
git checkout <branch-name>
``` 
 
  Switch to a branch.
   
```bash
git merge <branch-name>
```
 

Merge another branch into current.

   
```bash
 git diff <branch-name>
```
 
Show differences with a branch..
    
```bash
git branch -d <branch-name>
``` 
 
Delete a local branch.


## 🌱 Git Branching Concepts ##

### What is a Branch? ###  
   A Git branch is a parallel version of your project.It allows you to develop features, fix bugs, or experiment without affecting the main codebase. Branches 
   provide a safe and organized workflow for both individuals and teams.

#### Parent Branch #### 
   A parent branch is the original branch from which a new branch is created.
   * It acts as the base or starting point.
   * Typically, the main or develop branch serves as the parent.
   * Understanding parent branches helps prevent conflicts and improves  collaboration.

#### Child Branch ####
   A child branch is derived from another branch (the parent).
   * It contains all commit history from the parent up to the point of creation. 
   * Useful for isolated development of new features or fixes.
   * Changes from the child branch can be merged back into the parent branch when ready.

