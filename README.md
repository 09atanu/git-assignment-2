# 🌟 **A Complete Guide to Version Control** 🌟

Welcome to **Git Assignment 2**! 🎉 In this guide, we’ll walk you through **every step** using Git commands to complete your project. This hands-on approach will make you familiar with key Git concepts like branches, commits, and pull requests.

Let’s get started! 🚀

---

## 🚀 **Step 1: Create a New Directory and Initialize as Git Repository**

Before we can start working with Git, we need to create a new directory and initialize it as a Git repository. This is the foundation of our project.

```bash
mkdir git-assignment-2
cd git-assignment-2
git init
```

---

## 📝 **Step 2: Add a README.md File**

A **README.md** file provides information about your project. Let’s add one now!

```bash
echo "# Git Assignment 2" > README.md
```

---

## 📥 **Step 3: Make the Initial Commit**

Now that the `README.md` file is created, let’s commit it to the repository.

```bash
git add README.md
git commit -m "Initial commit with README.md"
```

---

## 🌍 **Step 4: Push the Repository to GitHub**

Next, we’ll push our project to GitHub to store it remotely and share it.

1. **Create a new repository** on GitHub (e.g., `git-assignment-2`).
2. Then, **push your local repository**:

```bash
git remote add origin https://github.com/09atanu/git-assignment-2.git
git push -u origin main
```

---

## 🔧 **Step 5: Create a New Branch - `feature-1`**

Let’s create a **new branch** called `feature-1` to start working on our first feature.

```bash
git checkout -b feature-1
```

---

## 🔄 **Step 6: Switch to `feature-1` Branch**

Make sure you’re on the `feature-1` branch. If not, you can switch to it:

```bash
git checkout feature-1
```

---

## ✏️ **Step 7: Make Changes to the Project**

We’re going to implement **feature-1** by creating a new file:

```bash
echo "This is feature 1 implementation" > feature-1.txt
```

---

## ✅ **Step 8: Commit the Changes**

Let’s commit the changes we just made.

```bash
git add feature-1.txt
git commit -m "Add feature-1 implementation"
```

---

## 🚀 **Step 9: Push the `feature-1` Branch**

Now, let’s push `feature-1` to GitHub.

```bash
git push -u origin feature-1
```

---

## 🔄 **Step 10: Create Another Branch - `feature-2`**

Now that `feature-1` is complete, let’s create `feature-2`.

```bash
git checkout main   # Switch to main
git pull origin main  # Update local main branch
git checkout -b feature-2  # Create and switch to feature-2 branch
```

---

## ✨ **Step 11: Make Changes for `feature-2`**

For `feature-2`, let’s add another implementation:

```bash
echo "This is feature 2 implementation" > feature-2.txt
git add feature-2.txt
git commit -m "Add feature-2 implementation"
```

---

## 🚀 **Step 12: Push the `feature-2` Branch**

Now, let’s push `feature-2` to GitHub as well:

```bash
git push -u origin feature-2
```

---

## 🔄 **Step 13: Create Pull Requests (PRs)**

It’s time to merge your features into the main branch! 🎉

1. **Create a pull request** (PR) for `feature-1` to `main`.
2. **Review** the changes and **merge** the PR.
3. **Repeat** the same for `feature-2`.

---

## 👀 **Step 14: Review Changes Before Merging**

Before merging, always review the PR changes:

- Check the **diffs** (changes) in the code.
- Leave any comments for improvements or clarifications.

---

## 🔧 **Step 15: Merge the PRs Sequentially**

To avoid any conflicts, merge **`feature-1` first**, followed by `feature-2`.

---

## ⚡ **Step 16: Keep Feature Branches Updated**

Before merging, make sure your feature branches are updated with the latest changes from `main`. You can do this by:

```bash
git checkout feature-1
git pull origin main  # Fetch the latest updates from main
git rebase main  # Rebase feature branch on top of main
git push --force  # Force push the rebased changes
```

---

## ⚠️ **Step 17: Resolve Conflicts During Rebase**

If conflicts arise during rebase, Git will notify you. Resolve them, and continue the rebase:

```bash
git add <resolved-files>
git rebase --continue
```

---

## 📅 **Step 18: Check Commit History in `main`**

Once both features are merged, let’s check the commit history to ensure everything is clean and linear.

```bash
git checkout main
git log --oneline
```

---

## 🧹 **Step 19: Delete Merged Branches**

After the merge is successful, let’s clean up by deleting the feature branches:

```bash
git branch -d feature-1  # Delete local feature-1 branch
git push origin --delete feature-1  # Delete remote feature-1 branch

git branch -d feature-2  # Delete local feature-2 branch
git push origin --delete feature-2  # Delete remote feature-2 branch
```

---

## 💡 **Final Commit and Submission**

We’ve completed the steps! Now let’s add all the Git commands used to the `README.md` file for easy reference:

```bash
echo "## Git Assignment 2 Commands" >> README.md
echo "1. git init" >> README.md
echo "2. git add README.md" >> README.md
echo "3. git commit -m 'Initial commit with README.md'" >> README.md
# Continue adding all commands similarly
```

---

### 📝 **Make the Final Commit**

Once the commands are added, **commit the changes** to the `README.md` file:

```bash
git add README.md
git commit -m "Add commands used for the Git assignment"
```

---

### 🌍 **Push the Final Changes**

Finally, **push** the updated `README.md` to GitHub:

```bash
git push origin main
```

---
### 📌 **Key Tips to Remember**:

- Always keep your branches updated with the main branch to avoid conflicts.
- Review PRs carefully before merging.
- Clean up your branches to keep the repository neat!

---
