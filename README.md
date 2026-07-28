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




