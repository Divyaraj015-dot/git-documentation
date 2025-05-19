

#  📗 Git Commands for Beginners #
A beginner-friendly guide to commonly used Git commands, complete with descriptions and key concepts. This documentation is structured for easy sharing and professional presentation.
## 🔧 Git Configuration ##
Set your global Git username.
```bash
git config --global user.name "Your Name"
```


Set your global Git email.
```bash
git config --global user.email "your-email@example.com"
``` 


## 🛠️ Repository Setup ##
 Initialize a new Git repository in the current directory.
```bash
git init
```
Clone a remote repository locally. 
 ```bash
git clone <repository-url>
```
 


Link your local repo to a remote one.   
```bash
git remote add origin <repository-url>
``` 
 




## 📄 Staging and Committing ##
Show changes and staged files. 
```bash
git status
``` 
 
 Stage one file for commit.
   
```bash
git add <filename>
``` 
Stage all changed files. 
 ```bash
git add .
```
 
 
Save staged changes with a message. 
```bash
git commit -m "your message"
```  
 

## ⬆️ Pushing and Pulling ##
  Push to remote main branch and track it.  
```bash
git push -u origin main
```
  

 Push committed changes to remote.   
```bash
git push
```  
  
 Fetch and merge changes from the remote repository.

```bash
git pull origin main
``` 
  


## 🌿Branch Management ##
 List local branches.
```bash
git branch
``` 
Create a new branch. 
```bash
git branch <branch-name>
```
 

 Switch to a branch.
```bash
git checkout <branch-name>
``` 
 


Merge another branch into current.   
```bash
git merge <branch-name>
```
 


Show differences with a branch.   
```bash
 git diff <branch-name>
```
 
Delete a local branch.

```bash
git branch -d <branch-name>
``` 
 



## 🌱 Git Branching Concepts ##

### What is a Branch? ###  
A Git branch is a parallel version of your project that allows you to develop features, fix bugs, or experiment without affecting the main codebase. It provides a safe and organized workflow for both individuals and teams.

#### Parent Branch #### 
A parent branch is the original branch from which a new branch is created.
* It acts as the base or starting point.
* Typically, the main or develop branch serves as the parent.
* Understanding parent branches helps prevent conflicts and improves collaboration.

#### Child Branch ####
A child branch is derived from another branch (the parent).
* It contains all commit history from the parent up to the point of creation. 
* Useful for isolated development of new features or fixes.
* Changes from the child branch can be merged back into the parent branch when ready.

