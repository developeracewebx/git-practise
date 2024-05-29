# Git Cheat Sheet

This README provides essential Git commands and procedures for common tasks. For a more comprehensive guide, refer to the official [Git Cheat Sheet](https://education.github.com/git-cheat-sheet-education.pdf).

## 1. How to Clone a Repository and Upload Code

### a) Clone the Project from GitHub:
1. Use the command:
   ```bash
   git clone <repo-path>

Replace <repo-path> with the URL of your repository. This command will clone the project from GitHub to your local machine.

## b) Upload Code from Local to GitHub:
 1. Ensure you are logged into your GitHub account in your editor (e.g., VS Code).
2. Check the status of your files:
    ```bash 
    git status
3. Add the files you want to commit:

   a) To add a single file:
   ```bash
   git add <file-path>
  b) To add all files:

    git add .

4. Commit your changes with a message:
    
    ```bash 
    git commit -m "Feat: worked on abc work"

5. Push the changes to GitHub:
    
    ```bash 
    git push

6. Check your GitHub repository to ensure your changes are there.



## 2. How to Clone a Repository and Upload Code

If two users are working on the same file and the first user has updated their code, the second user may encounter issues when trying to push their code.

   1. The second user can forcefully push their changes:

    git push -f <branch-name>

 Replace <branch-name> with the name of the branch.

2. When the first user tries to pull the code, they will receive an error:

        You have divergent branches and need to specify how to reconcile them.

3. To resolve this, the first user should use:

        git merge


This command will merge the changes from both users into the local branch. Resolve any conflicts manually.


## 3. How to Clone a Repository and Upload Code
a) Checkout to the Main Branch:

1. Use the command:
  
        git checkout main

b) Pull Latest Changes:

 1. Ensure your local main branch is up to date:
    
        git pull origin main


c) Create and Checkout the New Branch:

1. Create a new branch and switch to it:

        git checkout -b <new-branch-name>
        Replace <new-branch-name> with your desired branch name.

d) Push the New Branch to Remote:

1. Push the new branch to the remote repository:

        git push origin <new-branch-name>
        Replace <new-branch-name> with your new branch name.


## 3. How to Revert the Last Commit
If you need to revert the last commit that was pushed, you can use git revert. This creates a new commit that undoes the changes made by the last commit.

a) Revert the Last Commit:
 1. Use the command:
        
        git revert HEAD

b) In Nano:

1. Press Ctrl + O to write out (save) the file. Press Enter to confirm.
2. Press Ctrl + X to exit the editor.

c) Revert the Last Commit:
1. After saving and exiting, push the new revert commit to the remote repository:
        
        git push origin <your-branch>
        Replace <your-branch> with the name of your branch.

For a complete list of commands and detailed options, refer to the official "https://education.github.com/git-cheat-sheet-education.pdf".















