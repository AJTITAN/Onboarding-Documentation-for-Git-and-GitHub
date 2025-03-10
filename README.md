# Documentation for Git and GitHub Usage in ChaiCode Cohort !
# **Introduction** 
### Welcome to ChaiCode Cohort! This guide will help you get started with Git and GitHub, essential tools for managing code and collaborating with your team. 
### Whether you’re new to version control or looking for a refresher, this documentation covers the basics, setup, workflows, and best practices for working effectively within ChaiCode.
# **Basics of Git and GitHub**
## **What is Git ?**
### Git is basically a distributed version control system that allows developers to track changes in their code over time. It is used mainly for:
1. Keeping a history of code changes.
2. Collaboration among team members.
3. Branching and merging for feature development, fixing issues etc.
## **What is Github ?**
### GitHub is a platform that hosts Git repositories online, making collaboration easier. It provides tools for:
1. Code reviews and pull requests.
2. Issue tracking.
3. Continuous integration and deployment.
### GitHub provides third-party integrations with its vast marketplace of custom apps and actions thats why we are using github instead of other platforms like gitlab.

# Installation and Setup
## Installing Git
#### Windows

1. Download Git from [here](https://github.com/git-for-windows/git/releases/download/v2.47.1.windows.1/Git-2.47.1-64-bit.exe).
2. Run the installer and follow the setup wizard.
3. Verify the installation:
   ```bash
   git --version
   ```
#### macOS

1. Open the Terminal and install Git using Homebrew:
   ```bash
   brew install git
   ```
2. Verify the installation:
   ```bash
   git --version
   ```
#### Linux

1. Install Git using the package manager for your distribution:
   ```bash
   sudo apt install git   # Debian/Ubuntu
   sudo dnf install git   # Fedora
   ```
2. Verify the installation:
   ```bash
   git --version
   ```
### Configuring Git

Set your name and email to identify your commits:

```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```
![git user](photos/git%20user.png)

### Creating a GitHub Account

1. Go to [github.com](https://github.com/) and sign up.
2. Verify your email and set up two-factor authentication for security.

---

## Starting a New Repository

1. Navigate to your project folder.
2. Initialize a new Git repository:
   ```bash
   git init
   ```
   ![git init](photos/git%20init.png)
3. Add files to the repository:
   ```bash
   git add .
   ```
   ![git add](photos/git%20add.png)
4. Commit your changes:
   ```bash
   git commit -m "Initial commit"
   ```
   ![git commit](photos/git%20commit.png)

---

## Cloning any Repository from Github

1. Navigate to the GitHub repository you want to clone.
2. Copy the repository URL.
3. Clone the repository:
   ```bash
   git clone https://github.com/ChaiCode/example-repo.git
   ```
4. Navigate into the cloned repository:
   ```bash
   cd example-repo
   ```

---

## Basic Git Commands for work

- **Check Repository Status:**

  ```bash
  git status
  ```
  ![git status](photos/git%20status.png)

- **Stage Changes:**

  ```bash
  git add <file>
  git add .
  ```
  ![git add](photos/git%20add.png)

- **Commit Changes:**

  ```bash
  git commit -m "Your commit message"
  ```
  ![git commit](photos/git%20commit.png)

- **Push Changes to Remote Repository:**

  ```bash
  git push
  ```
  ![git push](photos/git%20push.png)

- **Pull Updates from Remote Repository:**

  ```bash
  git pull
  ```
  ![git pull](photos/git%20pull.png)

- **View Commit History:**

  ```bash
  git log
  ```
  ![git log](photos/git%20log.png)

---

## Commit Message Rules

Follow these guidelines for meaningful commit messages:

- Use the **present tense** (e.g., "Add feature").
- Capitalize the **first letter**.
- Keep messages **short** (50 characters or less).
- Use prefixes like `feat:`, `fix:`, `chore:`, `docs:`.

### Examples:

```bash
feat: Add tea selection feature
fix: Resolve login issue for tea enthusiasts
docs: Update README with chai varieties
```

---

## Branching Workflow

### Branch Strategy

ChaiCode uses the following branches:

- **main:** Production-ready code.
- **development:** Ongoing development.
- **feature/branch-name:** New features or fixes.

### Create and Switch Branches

1. Create a branch:
   ```bash
   git branch feature/tea-menu
   ```
   ![git new branch](photos/git%20branch.png)
2. Switch to the branch:
   ```bash
   git checkout feature/tea-menu
   ```
   ![git switching](photos/git%20switch.png)

### Merging Branches

1. Switch to the target branch (e.g., `main`):
   ```bash
   git checkout main
   ```
2. Merge the feature branch:
   ```bash
   git merge feature/tea-menu
   ```
   ![git merge](photos/git%20merge.png)
3. Resolve conflicts if any arise and commit the changes.

---

## Pull Requests (PR)

1. Push your branch to the remote repository:
   ```bash
   git push -u origin feature/tea-menu
   ```
   ![git pulling](photos/git%20pull%20branch.png)
2. Go to the repository on GitHub.
3. Click **New Pull Request** and select the source and target branches
4. Write a descriptive PR title and description.
5. Request a code review and submit the PR.

---

## Best Practices

1. **Commit Regularly:** Commit frequently to save your progress.
2. **Write Descriptive Commit Messages:** Make your changes clear to others.
3. **Pull Updates Regularly:** Stay updated with the latest changes to avoid conflicts.

---
We hope this guide helps you onboard quickly and efficiently. Welcome to the team at ChaiCode Cohort!
