#Introduction to Git and Its Core Commands

Objective: In this lesson, you will learn the basics of using Git, a distributed version control system, and understand the importance of its core commands. We will cover Git staging, committing changes, creating branches, and using pull requests for code review.

1. What is Git?
   - Git is a distributed version control system used for tracking changes in files and coordinating work among multiple developers.
   - It allows you to have a complete history of your project, including all changes made over time.

2. Setting up Git:
   - Install Git: Visit https://git-scm.com/downloads and download the appropriate version for your operating system.
   - Configure Git: Open a terminal or command prompt and set up your name and email using the following commands:
     ```
     git config --global user.name "Your Name"
     git config --global user.email "youremail@example.com"
     ```

3. Initializing a Git Repository:
   - To start using Git in your project, navigate to the project directory in your terminal and execute the following command:
     ```
     git init
     ```

4. Git Staging:
   - Before committing changes, you need to stage the files you want to include in the next commit using the following command:
     ```
     git add <file1> <file2> ...
     ```
     - Example: `git add index.html` (stages the "index.html" file)

5. Git Commit:
   - A commit records changes to your repository and creates a new point in the project's history. Use the following command to commit your staged changes:
     ```
     git commit -m "Commit message"
     ```
     - Example: `git commit -m "Added a new feature"`

6. Git Ignore:
   - Sometimes, you want to exclude specific files or directories from being tracked by Git. You can create a `.gitignore` file in your project's root directory and list patterns of files to ignore.
   - Example `.gitignore` file:
     ```
     # Ignore files with .txt extension
     *.txt

     # Ignore a directory named "logs"
     /logs/
     ```

7. Branches:
   - Git allows you to create branches, which are independent lines of development. They enable you to work on different features or bug fixes simultaneously without interfering with each other.
   - Creating a branch:
     ```
     git branch <branch-name>
     ```
     - Example: `git branch feature-branch` (creates a branch named "feature-branch")

   - Switching to a branch:
     ```
     git checkout <branch-name>
     ```
     - Example: `git checkout feature-branch` (switches to the "feature-branch" branch)

8. Pull Requests and Code Review:
   - Pull requests are a way to propose changes from a branch in your repository to the main branch. They facilitate code review and collaboration with other team members.
   - Steps to create a pull request:
     1. Push your branch to the remote repository:
        ```
        git push origin <branch-name>
        ```
     2. Visit the repository on a hosting platform (e.g., GitHub, GitLab) and locate your branch.
     3. Click on "New Pull Request" or a similar option and select the appropriate branches for comparison.
     4. Add a title, description, and reviewers for your pull request.
     5. Submit the pull request and wait for feedback and approval.

Conclusion:
Git is a powerful version control system that helps developers manage their codebase efficiently. Understanding core Git commands like staging, committing, branching, and pull requests is essential for effective collaborative development. By following these practices, you can maintain a well-documented history of your project and streamline the code review process.
