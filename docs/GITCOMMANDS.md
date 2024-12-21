# Git Commands for Initializing and Pushing to GitHub

This document provides a step-by-step guide to initialize a Git repository, commit changes, and push them to a GitHub repository.

## Step-by-Step Guide

1. **Initialize the Git Repository**
   ```bash
   git init
   ```
   This command initializes an empty Git repository in your project directory.

2. **Add All Files to Staging**
   ```bash
   git add .
   ```
   Use this command to add all files in the project directory to the staging area, preparing them for a commit.

3. **Commit the Changes**
   ```bash
   git commit -m "Initial commit - Gemini YouTube Analysis App"
   ```
   This commits the changes with a descriptive message.

4. **Rename the Default Branch to `main`**
   ```bash
   git branch -M main
   ```
   Rename the default branch to `main` to align with GitHub's default branch naming convention.

5. **Add the Remote Origin**
   ```bash
   git remote add origin https://github.com/<your-username>/<your-repo-name>.git
   ```
   Replace `<your-username>` and `<your-repo-name>` with your GitHub username and the repository name respectively.

6. **Push the Code to GitHub**
   ```bash
   git push -u origin main
   ```
   Pushes the code to the remote repository and sets `origin/main` as the tracking branch for future commits.

## Example

Here is an example sequence for a project named `GeminiYouTubeApp`:

```bash
# Initialize the repository
git init

# Add all files to staging
git add .

# Commit the changes
git commit -m "Initial commit - Gemini YouTube Analysis App"

# Rename the default branch to main
git branch -M main

# Add the remote origin
git remote add origin https://github.com/lhiebert01/GeminiYouTubeApp.git

# Push the code to GitHub
git push -u origin main
```

## Notes

- Ensure the GitHub repository is created **before** running these commands.
- The branch renaming step (`git branch -M main`) is critical to avoid errors like `src refspec main does not match any`.
- After the first push, you can simply use `git push` for subsequent updates.

---

Include this document in your technical documentation repository to ensure smooth Git operations.
