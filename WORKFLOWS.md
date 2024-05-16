# C++ Project Workflows

This document provides detailed workflows for creating and managing C++ projects, including how to link them with CLion and GitHub.

## Workflow 1: Create GitHub Repository First

### Steps

1. **Create a Repository on GitHub**:
    - Go to GitHub and create a new repository.
    - Initialize with a `README.md`, `.gitignore`, and a license if desired.

2. **Clone the Repository Locally**:
    - Open a terminal and clone the repository to your local machine:
      ```sh
      git clone https://github.com/your-username/repo-name.git
      cd repo-name
      ```

3. **Open the Project in CLion**:
    - Open CLion and select `Open` from the welcome screen.
    - Navigate to the cloned repository and open it.

4. **Create a New C++ Project**:
    - In CLion, create a new C++ project:
        - `File > New Project`
        - Select `C++ Executable` and configure the project settings.
        - Place the project in the cloned repository directory.

5. **Commit and Push Changes**:
    - Add, commit, and push the initial project setup to GitHub:
      ```sh
      git add .
      git commit -m "Initial project setup"
      git push origin main
      ```

## Workflow 2: Create Project in CLion First

### Steps

1. **Create a New C++ Project in CLion**:
    - Open CLion and create a new C++ project:
        - `File > New Project`
        - Select `C++ Executable` and configure the project settings.
        - Choose a directory to create the project in.

2. **Initialize a Git Repository Locally**:
    - Open the terminal in CLion or use an external terminal:
      ```sh
      cd /path/to/your/project
      git init
      git add .
      git commit -m "Initial commit"
      ```

3. **Create a Repository on GitHub**:
    - Go to GitHub and create a new repository.

4. **Link Local Repository to GitHub**:
    - Add the GitHub repository as a remote and push the local repository:
      ```sh
      git remote add origin https://github.com/your-username/repo-name.git
      git push -u origin main
      ```

## Workflow 3: Existing Project to GitHub

### Steps

1. **Open Existing Project in CLion**:
    - Open CLion and open your existing C++ project.

2. **Initialize a Git Repository Locally**:
    - Open the terminal in CLion or use an external terminal:
      ```sh
      cd /path/to/your/project
      git init
      git add .
      git commit -m "Initial commit for existing project"
      ```

3. **Create a Repository on GitHub**:
    - Go to GitHub and create a new repository.

4. **Link Local Repository to GitHub**:
    - Add the GitHub repository as a remote and push the local repository:
      ```sh
      git remote add origin https://github.com/your-username/repo-name.git
      git push -u origin main
      ```

## Additional Tips

- **Branching**: Use branches to manage different features or versions of your project.
- **Pull Requests**: Use pull requests to review and merge changes.
- **CI/CD**: Set up continuous integration and deployment to automate testing and building.

