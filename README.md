

#  📗 Git Commands for Beginners #
A beginner-friendly guide to commonly used Git commands, complete with descriptions and key concepts. This documentation is structured for easy sharing and professional presentation.
## 🔧 Git Configuration ##
1. Set your Git username
   
```bash
git config --global user.name "Your Name"
```


2. Set your Git email
   
```bash
git config --global user.email "your-email@example.com"
``` 


## 🛠️ Repository Setup ##
1. Initialize a new Git repo.
   
```bash
git init
```
2. Clone a remote repository locally.
   
 ```bash
git clone <repository-url>
```
 

3. Add remote repo
   
```bash
git remote add origin <repository-url>
``` 
 




## 📄 Staging and Committing ##
1. Show changes and staged files.
   
```bash
git status
``` 
 
2. Stage one file for commit.
   
```bash
git add <filename>
``` 
3. Stage all changed files.
   
 ```bash
git add .
```
 
 
4. Save staged changes with a message.
   
```bash
git commit -m "your message"
```  
 

## ⬆️ Pushing and Pulling ##
1. Push to main branch with tracking.
   
```bash
git push -u origin main
```
  

2. Push committed changes to remote.
     
```bash
git push
```  
  
3. Fetch and merge remote changes.

```bash
git pull origin main
``` 
  


## 🌿Branch Management ##
1. List local branches.
   
```bash
git branch
``` 
2. Create a new branch.
   
```bash
git branch <branch-name>
```
 

3. Switch to a branch.
   
```bash
git checkout <branch-name>
``` 
 


4. Merge another branch into current.
    
```bash
git merge <branch-name>
```
 


5. Show differences with a branch.
     
```bash
 git diff <branch-name>
```
 
6. Delete a local branch.

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

#### ❓What is the origin/main? ####
   In git origin and main have specific meanings:
 1. origin
 * origin is the default name Git gives to the remote repository you cloned your project from.

 * It acts as a shortcut so you don’t have to type the full URL every time you push or pull code.

   We can think of it as:
   origin = remote location of the project.
   Example:

```bash

git clone https://github.com/username/repo-name.git
```
   After cloning, Git automatically sets origin as the reference to https://github.com/username/repo-name.git.


 2. main
 * main is the default branch name in many new GitHub repositories (previously, master was the default).

 * It is usually the primary working branch where the latest stable version of the code lives.
 * This is the branch name we are pushing to.

   Together: origin/main
   origin/main refers to the main branch of the remote repository (i.e., the main branch on GitHub, not your local one).

   If we run:

```bash

git fetch
git log origin/main
```
It shows the commit history of the remote main branch.

