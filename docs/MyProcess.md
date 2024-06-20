# GitHub Workflow Guide

This guide provides step-by-step instructions for managing a GitHub repository, including cloning, forking, branching, merging, handling conflicts, enabling GitHub Pages, and exploring open-source projects. Follow these tasks to familiarize yourself with GitHub and Git commands.

## Requirements

- A GitHub account ([create one here](https://github.com/)).
- Git installed on your local machine ([download Git](https://git-scm.com/)).
- A code editor of your choice (e.g., [Visual Studio Code](https://code.visualstudio.com/), [Sublime Text](https://www.sublimetext.com/)).

## Task 1: Cloning and Forking

### 1. Cloning a Repository

1. **Choose a Repository:**
   - Select a public GitHub repository of interest.
   - Example: `https://github.com/user/repository`

2. **Clone the Repository:**
   ```sh
   git clone https://github.com/user/repository.git
   cd repository
   ```

3. **Explore the Repository:**
   - Navigate through the directory structure.
   - Review files and their contents.
   - Examine the commit history:
     ```sh
     git log
     ```

### 2. Forking a Repository

1. **Fork the Repository:**
   - Go to the GitHub page of the selected repository.
   - Click the "Fork" button in the top right corner.

2. **Clone the Forked Repository:**
   ```sh
   git clone https://github.com/your-username/repository.git
   cd repository
   ```

## Task 2: Managing Branches

### 3. Creating and Switching Branches

1. **Create a New Branch:**
   ```sh
   git checkout -b feature-update
   ```

2. **Switch to the Branch:**
   ```sh
   git checkout feature-update
   ```

### 4. Making Changes and Committing

1. **Make Changes:**
   - Edit an existing file or add a new file.

2. **Commit the Changes:**
   ```sh
   git add .
   git commit -m "Describe your changes"
   ```

### 5. Merging Changes

1. **Switch to the Main Branch:**
   ```sh
   git checkout main
   ```

2. **Merge the Changes:**
   ```sh
   git merge feature-update
   ```

## Task 3: Handling Conflicts

### 6. Creating Conflicts

1. **Make Conflicting Changes:**
   - In your forked repository, edit the same file modified in Task 4.
   - Commit the changes.

### 7. Resolving Conflicts

1. **Create a New Branch for Conflict Resolution:**
   ```sh
   git checkout -b conflict-resolution
   ```

2. **Resolve the Conflict Manually:**
   - Open the conflicted file and edit as necessary.
   - Mark resolved conflicts and save the file.

3. **Commit the Changes:**
   ```sh
   git add .
   git commit -m "Resolved conflict"
   ```

4. **Merge the Conflict-Resolution Branch:**
   ```sh
   git checkout main
   git merge conflict-resolution
   ```

## Task 4: GitHub Pages

### 8. Enabling GitHub Pages

1. **Create an HTML File:**
   - Create a file named `index.html` with some content.
   
2. **Push the Changes:**
   ```sh
   git add index.html
   git commit -m "Add index.html for GitHub Pages"
   git push origin main
   ```

3. **Enable GitHub Pages:**
   - Go to the repository on GitHub.
   - Navigate to `Settings > Pages`.
   - Set the source branch to `main` and save.

### 9. Accessing the Published Page

1. **Visit the GitHub Pages URL:**
   - The URL will typically be `https://your-username.github.io/repository`.
   - Verify that the `index.html` content is displayed.

