

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

   * It acts as a shortcut so we don’t have to type the full URL every time we push or pull code.

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
 
 #### 🤔 Why is it necessary to set the origin for a New Branch? ####
 
 When we create a new branch locally using Git, it exists only on our computer. For others (or GitHub) to know about this branch, we need to push it to the 
 remote repository (usually named origin).

💡 So, setting or using origin is necessary to:
 * Publish the branch to GitHub.

 * Enable collaboration (so others can pull/merge your branch).

 * Track changes between your local branch and the remote version.

#### ❓How to set the origin for a New Branch? ####

   When we create a new branch locally, Git doesn't automatically know where to push it on GitHub. We need to set the origin so our local branch connects to the 
   remote one.

   🛠️ Step-by-Step Guide
   1️⃣ Create a New Branch Locally
```bash

git checkout -b feature/my-new-branch
```
  This creates a branch called feature/my-new-branch only on your computer.

  2️⃣ Push the Branch to GitHub & Set the Origin
```bash

git push -u origin feature/my-new-branch
```
  ✅ What each part means:
  * push: Sends your branch to GitHub.

  * -u or --set-upstream: Links your local branch to the remote one.

  * origin: The name of your remote repo (usually GitHub).

  * feature/my-new-branch: Your new branch name.

 3️⃣ After That, It's Easy!
  Once linked, you can simply use:

```bash

git push
```
or

```bash

git pull
```
  and Git knows which remote branch to use—no need to type the full command again.

🔍 How to Check If the Origin Is Set
```bash

git branch -vv
```
This shows all your branches and their tracking info.

## 🧵 What is git stash? ##

git stash is a Git command used to temporarily save our uncommitted changes (both staged and unstaged) without committing them. It allows us to switch branches or work on something else without losing our current progress.

### ✨ Why Use git stash? ###
   * We're in the middle of some work.

   * We need to switch to another branch to fix a bug or test something.

   * We don’t want to commit your partial work yet, but also don’t want to lose it.

#### 📌 Basic Stash Commands ####
🔹 Save current changes

  
```bash

git stash
#Temporarily saves your changes and gives you a clean working directory.
```
   

🔹 See a list of stashed items

   
```bash

git stash list
#Displays all saved stashes.
```
   

  #Example output:

```bash
stash@{0}: WIP on main: 1a2b3c4 updated about section
```
🔹 Apply the latest stash (and keep it) 

 
```bash


git stash apply
#Restores your saved changes into the current working directory.
```
 

🔹 Apply and remove the stash

  
```bash
 
git stash pop
#Restores the changes and removes the stash from the list.
```


🔹 View changes inside a stash 


```bash

git stash show -p
#Shows the detailed diff of the most recent stash.
```
  

🔹 Delete a specific stash
```bash

git stash drop stash@{0}
#Deletes one specific stash from the list.
```


🔹 Delete all stashes
 
```bash

git stash clear
#Removes all saved stashes.
```
.

🧪 Example Workflow
```bash

# Step 1: Edit a file (e.g., about.html)


# Step 2: Save uncommitted changes
git stash

# Step 3: Do something else (like switching branches)
git checkout main

# Step 4: Return to the original branch
git checkout feature/about-page

# Step 5: Reapply your saved work
git stash apply

# Step 6: (Optional) Remove the stash
git stash drop
💡 Undo Stash Apply
```
If you apply a stash and then want to discard the changes (go back to the last commit):

``` bash

git restore <filename>

# Example:
git restore about.html
```




