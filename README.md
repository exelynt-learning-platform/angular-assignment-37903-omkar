# angular-assignment-37903-omkar

Understanding Version Control, Git, and GitHub Fundamentals
1. What is Version Control and Why is it Important?

Version control is a system used to track changes made to files, documents, and source code over time. It allows developers to save different versions of their work and see what changes were made, when they were made, and sometimes who made them.

Version control is important because it helps developers avoid losing their work and makes it possible to return to an earlier version if something goes wrong. It is especially useful when multiple developers are working on the same project because everyone can work on the project without accidentally overwriting each other's changes.

For example, if a developer makes a change that causes an application to stop working, version control allows them to check previous versions and restore a working version.

2. Why Do Developers Use Git?

Git is a popular distributed version control system that developers use to manage and track changes in their code.

Developers use Git because it provides several useful features:

It keeps a history of changes made to a project.
Developers can create branches to work on new features without affecting the main code.
Multiple developers can work on the same project at the same time.
Changes can be reviewed before they are added to the main project.
Developers can go back to an earlier version when needed.
Git works locally, so developers can make commits without always needing an internet connection.

Git makes software development more organized and helps teams collaborate safely and efficiently.

3. Common Problems Git Solves

Git solves many common problems that developers face when working individually or in teams.

Losing Previous Work

Git stores a history of changes, so developers can restore earlier versions of their code if necessary.

Overwriting Other Developers' Work

When multiple developers work on the same project, Git helps combine their changes and identifies conflicts when two people modify the same part of a file.

Working on Multiple Features

Developers can create separate branches for different features or bug fixes. This allows them to work independently without affecting the stable version of the project.

Tracking Changes

Git records who made changes and what was changed. This makes it easier to understand the development history of a project.

Recovering from Mistakes

If a new change introduces a bug, developers can compare changes, undo them, or return to a previous working version.

Team Collaboration

Git provides a structured way for developers to share their work, review changes, and combine contributions from different team members.

4. Difference Between Git and GitHub

Git and GitHub are related, but they are not the same thing.

Git is a version control system and software that runs on a developer's computer. It is used to track changes in code, create branches, make commits, and manage different versions of a project.

GitHub is a cloud-based platform that provides online hosting for Git repositories. It allows developers to store their Git projects online and collaborate with other people.

For example, a developer can use Git on their computer to create commits and branches. They can then use GitHub to upload and share the project with their team.

In simple terms:

Git = Tool for version control
GitHub = Online platform for hosting and collaborating on Git repositories

Git can be used without GitHub, and GitHub primarily uses Git to manage repositories.

5. Centralized vs Distributed Version Control Systems

There are two common types of version control systems: Centralized Version Control Systems (CVCS) and Distributed Version Control Systems (DVCS).

Feature	Centralized Version Control	Distributed Version Control
Repository	Usually one central repository	Every developer has a complete repository
Internet/Network	Often requires connection to the central server	Many operations can be performed offline
Example	SVN, CVS	Git, Mercurial
Failure Risk	Central server can become a single point of failure	Multiple complete copies reduce this risk
Collaboration	Developers depend more on the central server	Developers can work independently and share changes later
Speed	Some operations depend on the network	Many operations are fast because they happen locally
Centralized Version Control

In a centralized system, there is one main repository stored on a central server. Developers connect to this server to get the latest code and submit their changes.

The main advantage is that the project is managed from one central location. However, if the central server is unavailable, developers may not be able to perform many operations. It can also create a single point of failure.

Distributed Version Control

In a distributed system, each developer has a complete copy of the repository, including its history. Developers can commit changes and create branches locally without always needing a connection to a central server.

Git is a distributed version control system. Developers can work independently and later share their changes with others through a remote repository such as GitHub.


## Git Installation & Setup

Git was successfully installed and verified using the `git --version` command.

The global Git username and email were configured and verified using Git configuration commands.

A Git repository was also initialized using `git init`, and the repository status was checked using `git status`.

### Screenshot

<img width="1512" height="907" alt="Screenshot 2026-07-28 at 12 32 28 PM" src="https://github.com/user-attachments/assets/7bb91152-4ad0-4010-b4c8-98f0202f2aa4" />
<img width="1512" height="907" alt="Screenshot 2026-07-28 at 12 32 16 PM" src="https://github.com/user-attachments/assets/8b1a1b5c-3434-42f4-8f38-61443e974933" />


## Create and Understand a Git Repository

### 1. Create a New Project Folder
I created a new project folder named `git-repository-assessment`.

### 2. Initialize Git Repository
I initialized the project using `git init`. This created the `.git` folder, which stores Git's internal repository information, including commit history, branches, and configuration.

### 3. Create a New File
I created `index.txt` using `touch index.txt`.

### 4. Check File Status
I used `git status` to check the repository status. Initially, `index.txt` appeared as an untracked file.

### 5. Add File to Staging Area
I used `git add index.txt` to move the file to the staging area.

### 6. Commit the File
I committed the staged file using:

`git commit -m "Initial commit"`

### 7. Final Status
I ran `git status` and confirmed:

`nothing to commit, working tree clean`

This confirms that the file was successfully committed.

### Three Git File States

- **Working Directory:** Where files are created and modified.
- **Staging Area:** Where changes are prepared for the next commit using `git add`.
- **Git Repository:** Where committed changes are stored in Git history.

### Git Workflow

Working Directory → `git add` → Staging Area → `git commit` → Git Repository

<img width="1512" height="907" alt="Screenshot 2026-07-28 at 12 50 48 PM" src="https://github.com/user-attachments/assets/8cd398af-baea-47ff-8f63-fa646f0e9650" />

## Tracking and Committing Changes in Git

### Overview

In this task, I practiced tracking files and committing changes using Git.

I created two files, `file1.txt` and `file2.txt`, and checked their status using `git status`. I staged each file using `git add` and committed them separately with meaningful commit messages.

### Git Commands Used

git status
git add file1.txt
git commit -m "Add first project file"

git add file2.txt
git commit -m "Add second project file"

git log --oneline


2. Create Files

I created two new files named file1.txt and file2.txt:

touch file1.txt file2.txt

I then used git status to check the repository. Git identified both files as untracked files.

3. Stage and Commit the First File

I added file1.txt to the staging area using:

git add file1.txt

I then committed the staged file with a meaningful commit message:

git commit -m "Add first project file"

This created the first commit for the task.

4. Stage and Commit the Second File

I added file2.txt to the staging area:

git add file2.txt

I then created another commit:

git commit -m "Add second project file"

This created a second commit and demonstrated how Git tracks changes through multiple commits.

5. View Commit History

I viewed the commit history using:

git log --oneline

The command displayed the commit history in a concise format. It confirmed that multiple commits were successfully created with meaningful commit messages.

6. Common Beginner Mistakes
Mistake 1: Forgetting to Stage Changes

A common beginner mistake is trying to commit changes without first adding them to the staging area.

For example:

git commit -m "Update files"

If the changes have not been staged, Git will not include them in the commit.

Solution:

First stage the changes:

git add <filename>

Then create the commit:

git commit -m "Meaningful commit message"
Mistake 2: Using Unclear Commit Messages

Another common mistake is using unclear commit messages such as update, changes, or test. These messages do not explain what was changed.

Solution:

Use clear and meaningful commit messages that describe the change, for example:

git commit -m "Add user authentication validation"

Meaningful commit messages make the project history easier to understand and help developers identify changes quickly.

Conclusion

Through this task, I learned how to check file status using git status, stage changes using git add, create commits using git commit, and view commit history using git log --oneline. I also learned the importance of using meaningful commit messages and avoiding common Git mistakes.


<img width="1512" height="907" alt="Screenshot 2026-07-28 at 1 03 39 PM" src="https://github.com/user-attachments/assets/01fbc030-9572-4c13-b4d6-f6e638124180" />



## Merge Conflicts

A merge conflict occurs when Git cannot automatically combine changes from two branches. This usually happens when two branches modify the same lines of the same file in different ways.

For example, if the `main` branch and a feature branch both modify the same line in a file, Git cannot decide which change should be kept. Git marks the file as conflicted and requires the developer to resolve it manually.

### Steps to Resolve a Merge Conflict

1. Run the merge command.
2. Open the file containing the conflict.
3. Check the conflict markers:
   - `<<<<<<< HEAD`
   - `=======`
   - `>>>>>>> branch-name`
4. Decide which changes should be kept.
5. Remove the conflict markers.
6. Save the file.
7. Stage the resolved file using `git add`.
8. Commit the resolved changes using `git commit`.

Merge conflicts are common when multiple developers work on the same files or when different branches contain conflicting changes.

<img width="1512" height="907" alt="Screenshot 2026-07-28 at 1 15 13 PM" src="https://github.com/user-attachments/assets/b88b1978-c2bb-46bf-985f-e5d76cbda93f" />


## Getting Started with GitHub and Remote Repositories

### 1. GitHub Account

I created and configured a GitHub account to manage my Git repositories and collaborate with other developers.

### 2. Remote Repository

A remote repository was created on GitHub to store the project code and maintain the project history remotely.

### 3. Connecting Local Repository to GitHub

The local Git repository was connected to the GitHub remote repository using the `git remote add origin` command.

Example:

git remote add origin <repository-url>

<img width="1512" height="907" alt="Screenshot 2026-07-28 at 1 21 37 PM" src="https://github.com/user-attachments/assets/c69876b2-5103-49a5-8ffd-1a48def608c9" />


## Managing Code with Remote Git Repositories

### 1. Git Push

The `git push` command uploads local commits to a remote Git repository such as GitHub.


<img width="1512" height="907" alt="Screenshot 2026-07-28 at 3 31 15 PM" src="https://github.com/user-attachments/assets/3cab5752-8d77-4b2e-b3cf-79d1d9f1ee0b" />
<img width="1512" height="907" alt="Screenshot 2026-07-28 at 3 31 24 PM" src="https://github.com/user-attachments/assets/2c476750-ca92-4446-b49a-f2ba36362b99" />


# GitHub Collaboration and Best Practices

## Project Overview

This repository demonstrates basic GitHub collaboration workflows and Git best practices for React projects.

The purpose of this assignment is to understand how developers collaborate using Git and GitHub while maintaining a clean, organized, and maintainable project repository.

---

## Repository Structure


git-repository-assessment/
├── .gitignore
├── README.md
└── src/
    ├── components/
    ├── pages/
    ├── services/
    ├── hooks/
    └── utils/


---

## GitHub Workflow

A basic GitHub workflow for a React project is:

1. Clone the repository.
2. Create a new feature branch.
3. Make changes and test them locally.
4. Check the changes using `git status`.
5. Stage the changes using `git add`.
6. Commit the changes with a meaningful commit message.
7. Push the branch to GitHub.
8. Create a Pull Request.
9. Review the changes.
10. Merge the Pull Request into the main branch.

Example:


git clone <repository-url>
git checkout -b feature/my-feature
git add .
git commit -m "feat: add new feature"
git push origin feature/my-feature



## Assignment Execution Evidence
### 1. Git Branches and Repository Status
### 2. Git Commit History
### 3. Feature Branch Creation and Merge
### 4. Remote Repository Configuration
### 5. GitHub Repository
### 6. Final Main Branch and Remote Synchronization

<img width="1512" height="907" alt="Screenshot 2026-07-28 at 4 00 32 PM" src="https://github.com/user-attachments/assets/ad6ad87c-a840-4c95-ba49-61a5d20e43db" />
<img width="1512" height="907" alt="Screenshot 2026-07-28 at 4 00 51 PM" src="https://github.com/user-attachments/assets/e1ea2caf-5ffe-4549-bc47-4df6bc93dab2" />
<img width="1512" height="907" alt="Screenshot 2026-07-28 at 4 01 34 PM" src="https://github.com/user-attachments/assets/8a63da08-e7fa-474e-802d-de2a91d593d7" />
<img width="1512" height="907" alt="Screenshot 2026-07-28 at 4 01 53 PM" src="https://github.com/user-attachments/assets/9ee505ca-123d-4491-9c49-f163ca065daf" />




