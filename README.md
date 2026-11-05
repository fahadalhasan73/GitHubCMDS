# GitHubCMDS
In this repository I am storing the essential commands for git and github

## How to upload a folder from local PC to GitHub
### Step 01:
Create a new GitHub Repository (Same as the folder name recommended). Github will show a URL like "https://github.com/fahadalhasan73/level2Batch8.git". Need to store it
### Step 02:
Initialize Git in local folder. 
Code: git init
This creates a hidden .git directory inside level2Batch8(Folder). It allows Git to start tracking the project history.
Next run: git status
This should display information about the current branch and untracked files, if any.



## How to push an edited/modified file from local PC to GitHub

```TypeScript
git status
git add .
git commit -m "Add teaching materials and update styles"
git push
```

Modify (Files) -> Stage (git add) -> Commit (git commit) -> Push (git push) 


### Step 02: Check what has changed
```powershell
git status
```
We can also inspect tracked-file edits using:
```powershell
git diff
```
### Step 03: Stage the changes
Now we need to tell Git which changes should go into the next commit. We will have two choices  
**Option A: Stage everything (convenient for small projects)**  
```powershell
git add .
```
This stages eligible new, modified, and deleted files under the current directory.  
**Option B: Stage specific files (better when you have unrelated changes)**  
```powershell
git add index.html
git add images/
```
This stages only the specified file and the files inside the new folder.  
Reasoning: Staging separates everything we've edited from what we actually want to save in the next commit.  
For example, imagine we modified five files but only want to commit two. Git lets us stage only those two.  
After staging we can check the updated status using
```powershell
git status
```
Note: Git tracks files, not empty folders.  

### Step 04: Create a commit
```powershell
git commit -m "Add logo and update homepage (Message actually)"
```
A commit records a snapshot of your staged changes in the local Git repository.  
A commit includes a unique hash, the author, timestamp, message, and references to the saved project snapshot and previous history.  
Important: After committing, New changes are saved in Git locally, but they are not yet uploaded to GitHub. We can create several commits locally before pushing them together.  

### Step 05: Push the commit to GitHub
```powershell
git push
```






























