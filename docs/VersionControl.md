## Source Code Version Control Tools

### Introduction
Version control is an essential part of software development, enabling developers to manage changes to their codebase efficiently. It facilitates collaboration, maintains the integrity and history of the project, and helps in tracking and combining contributions from different team members. This document outlines our approach to version control within the context of our Flutter application development, targeting both web and future mobile deployments.

### Version Control System Used
For our project, we have chosen **Git** as our version control system (VCS), in conjunction with **GitHub** for online hosting of the repository. Git was selected for its widespread adoption, flexibility, and powerful branching and merging capabilities. Additionally, GitHub provides an intuitive platform for code review, collaboration, and integration with various development tools, enhancing our CI/CD pipeline's efficiency.

### Repository Setup
#### Structure
Our repository employs a feature-based branching strategy, separating production, development, and feature branches to maintain a clean and functional codebase. The directory layout is organized according to Flutter's best practices to ensure that the project is easily navigable and scalable.

### Repository Setup
#### Structure
Our repository employs a feature-based branching strategy, separating production, development, and feature branches to maintain a clean and functional codebase. The directory layout is organized as follows:

- `/.devcontainer`: Contains the recommended development environment configuration files. This ensures that all team members use a consistent environment, which reduces the "it works on my machine" problem.

- `/docs`: This directory hosts all project documentation, ensuring that design documents, setup instructions, and other important information are easily accessible and well-organized.

- `/app`: Houses the Flutter application source code. This separation ensures that the application code remains isolated from documentation and other non-app-related files, facilitating a clearer workflow and easier navigation.

- `/.github/workflows`: Contains the automated GitHub Actions definition files. These files define our continuous integration and delivery pipeline, automating tests, builds, and deployments based on predefined events and conditions.

This structured approach enhances our project’s navigability and scalability, aligning with Flutter's best practices and supporting our agile development methodologies.


#### Integration
The repository is integrated with our DevContainer and CI/CD pipeline, ensuring that every push triggers automated tests and builds, facilitating continuous integration and delivery. This setup supports our agile development practices and enhances code quality.

#### Standards and Conventions
We enforce specific standards for commit messages and branch naming conventions to maintain a clear and informative project history. For example, commit messages must include a brief description of changes and a reference to the related task or issue. Branch names should reflect the feature or bug fix they are addressing.

### Common Commands and Usage
Below are common Git commands used in our project workflow:

- `git clone <repository-url>`: Clones the repository to your local machine.
- `git branch <branch-name>`: Creates a new branch.
- `git checkout <branch-name>`: Switches to a specified branch.
- `git add .`: Stages all changes for commit.
- `git commit -m "Commit message"`: Commits the staged changes with a descriptive message.
- `git push origin <branch-name>`: Pushes the commits to the remote repository.
- `git merge <branch-name>`: Merges the specified branch into the current branch.
- `git pull`: Updates the local repository to the latest changes from the remote.

### Collaboration Features
GitHub enhances collaboration through features like pull requests and code reviews, allowing team members to propose, discuss, and review changes before they are merged into the main codebase. The platform also supports conflict resolution directly in the web interface, simplifying the process of integrating different changesets.

### Challenges and Solutions
See the [project issues](https://github.com/derek-munday/PrisonersDilemmaExperiment/issues) section for active and historical issues.

### Conclusion
Adopting Git and GitHub has significantly improved our project's organization, collaboration, and overall code quality. The integration of version control into our development workflow has not only streamlined the process but also provided a reliable and scalable framework for managing our application's lifecycle. Through this experience, we've gained valuable insights into the importance of effective version control practices in modern software development.

