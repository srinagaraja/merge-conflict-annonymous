# merge-conflict-annonymous
A safe space to learn and resolve conflicts 🧘

Use this dummy repo as you want to practice your git skills. Or you could follow the following instructions for a tutorial on basic git commands.

# Git Tutorial

## Challenge 1: Create a Branch & Commit Changes in `contributors.txt`

**Goal**: Learn how to create a branch, add a file, and commit changes.

**Steps:**

1. Clone the repository:
   ```bash
   git clone https://github.com/srinagaraja/merge-conflict-annonymous.git
   ```
2. Create a new branch:
   ```bash
   git checkout -b yourname_feature
   ```
3. Add your name to `contributors.txt` If you wish do via bash:
   ```bash
   echo "Your Name" >> contributors.txt
   ```
4. Stage and commit the change:
   ```bash
   git add contributors.txt
   git commit -m "Added my name to contributors.txt"
   ```
5. Push the branch to GitHub:
   ```bash
   git push origin add-contributor
   ```
**Note**: While working in open source projects, before cloning you fork the repo to your github. Then you proceed to clone the forked repo. This ensures that the changes you make after committing is only happening in the forked repo. You might need permissions (approved pull requests) to make changes in the main project.  
**Outcome**: You have created a new branch and committed your changes.

---

## Challenge 2: Switch Between Multiple Branches

**Goal**: Learn how to navigate between different branches.

**Steps:**

1. List all branches:
   ```bash
   git branch
   ```
2. Switch to a different branch:
   ```bash
   git checkout yourname_feature
   ```
3. Return to the `main` branch:
   ```bash
   git checkout main
   ```

**Outcome**: You can now move between branches effectively. And notice how the changes you made are only visible in your branch!


## Challenge 3: Use Case for `git stash`

**Goal**: Learn how to temporarily save changes without committing them.

**Steps:**

1. Make changes to a file but **don’t commit**:
   ```bash
   echo "My favourite colour is..." >> contributor.txt
   ```
   Hold on! There are some issues in the python script that needs your immidiate attention. 
2. Stash the changes:
   ```bash
   git stash
   ```
3. Verify that the working directory is clean:
   ```bash
   git status
   ```
4. Make changes in the file (follow the comments or erase the error. Just make some change in the file). Add and commit these changes.
4. Retrieve stashed changes:
   ```bash
   git stash pop
   ```

**Outcome**: You understand how to pause and resume work without committing. If you want to commit the changes you made in the stash you have to pop it first and then commit (stage always before commit!!!)

---

## Challenge 5: `git blame` Use Case

**Goal**: Learn how to track changes and identify contributors.

**Steps:**

1. Run `git blame` on a file:
   ```bash
   git blame contributors.txt
   ```
2. Identify who made a specific change.


**Outcome**: You can trace the history of a file to understand past changes.

---

## Challenge 6: Remove a File but Keep Its History (`git rm`)

**Goal**: Learn how to remove files while keeping them in Git history.

**Steps:**

1. Remove `old-notes.txt` from the repo:
   ```bash
   git rm old-notes.txt
   ```
2. Commit and push the change:
   ```bash
   git commit -m "Removed old-notes.txt from the repo"
   git push origin yourname_feature
   ```
3. Restore it later from history if needed:
   ```bash
   git checkout HEAD~1 old-notes.txt
   ```

**Outcome**: You understand how to remove a file from the project but keep its history.

---

## Challenge 7: Time Travel with `git checkout`

**Goal**: Learn how to check out previous versions of a file.

**Steps:**

1. View commit history:
   ```bash
   git log --oneline
   ```
2. Checkout an old commit:
   ```bash
   git checkout <commit-hash>
   ```
3. View the state of the project at that time.
4. Return to the latest version:
   ```bash
   git checkout yourname_feature
   ```

**Outcome**: You can view and retrieve old versions of your project.

---


## Final Task: Submit a Pull Request

Each participant should submit a **Pull Request** to merge their changes into the main repository! 🚀

## Final_Final Task: Pull to local
```bash
   git pull origin main

   ```
Substitue main with branch_name incase you want to pull from your working branch.
## Final_Final_I_Swear Task: Delete the branch
```bash
   git branch -d yourname_feature

   ```


