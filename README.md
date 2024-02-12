# WIKI PAGE IS CREATED FOR THE DEVOPS ASSIGNMENT! (click [here](https://github.com/cybermad7373/73772126145-DevOps-Assignment1/wiki) )
# Git Operations Demonstration

This repository demonstrates various Git operations using both local and remote (GitHub) repositories. Screenshots of the demonstration are not provided here, but you can follow the instructions to perform these operations on your local and remote repositories.

## 1. Git Clone

The `git clone` command is used to create a local copy of a Git repository. Execute the following syntax:

```bash
git clone <repository_URL>
```

Replace `<repository_URL>` with the actual URL of the Git repository.

## 2. Git Push

The `git push` command uploads local changes to a remote Git repository. For example:

```bash
git push origin main
```

This pushes changes from the local "main" branch to the "main" branch on the remote repository named "origin."

## 3. Git Pull

The `git pull` command fetches and integrates changes from a remote repository into the current branch. Example:

```bash
git pull origin main
```

This fetches changes from the "main" branch on the remote repository named "origin" and integrates them locally.

## 4. Git Reset

The `git reset` command resets the current branch to a specific commit or undoes changes in the working directory.

```bash
git reset --hard <commit_hash>
```

Replace `<commit_hash>` with the commit hash to which you want to reset.

## 5. Git Commit

The `git commit` command is used to save changes to the local repository.

```bash
git commit -m "Your commit message"
```

Write a descriptive commit message explaining your changes.

## 6. Git Log

The `git log` command displays the commit history of a repository.

```bash
git log
```

This shows commit information, including hash, author, date, and commit message.

## 7. Git Status

The `git status` command displays the current status of your working directory in relation to the Git repository.

```bash
git status
```

Check the status of your changes, including modified, staged, and untracked files.

## 8. Git Stash

The `git stash` command temporarily saves changes not ready to be committed.

```bash
git stash
```

This allows you to switch branches or perform other tasks without committing the changes.

## 9. Pull Request

To create a pull request, make changes in a feature branch, push the branch to the remote repository, and use the hosting platform's interface (e.g., GitHub) to initiate the pull request for code review and merging.

## 10. Branching & Merging Commands

For branching and merging in Git, use commands like `git branch`, `git checkout` or `git switch`, `git merge`, and handle conflicts with `git add` and `git commit`.

## 11. Branch Protection Rules & Merge Conflicts

Enforce branch protection rules on the hosting platform to prevent direct pushes, require pull requests, and manually resolve merge conflicts using `git add` and `git commit`.

Feel free to refer to the individual sections for detailed instructions on each Git operation.
```

Make sure to replace placeholders such as `<repository_URL>` and `<commit_hash>` with your actual repository URL and commit hash. This README serves as documentation for users or collaborators on your project.
```

# Jenkins Pipeline Project - Display Student Details

This repository demonstrates a Jenkins pipeline project to display student details using the `echo` command. Follow the steps below to set up and run the pipeline.

## Steps

### 1. Create a Pipeline Project

- Open Jenkins and create a new pipeline project.

### 2. Write a Pipeline Script

- In the pipeline configuration, use the following script:

```groovy
pipeline {
    agent any
    
    stages {
        stage('Display Student Details') {
            steps {
                echo 'Student Details:'
                echo "a) Register Number: <your_register_number>"
                echo "b) Name: <your_name>"
                echo "c) Department: <your_department>"
                echo "d) Year: <your_year>"
                echo "e) Area of Specialization: <your_specialization>"
            }
        }
    }
}
```

Replace `<your_register_number>`, `<your_name>`, `<your_department>`, `<your_year>`, and `<your_specialization>` with your actual student details.

### 3. Build the Project

- Save the pipeline configuration and trigger a build.

### 4. Output

- View the console output of the build to see the displayed student details.

## Note

- This pipeline project is a simple demonstration using the `echo` command to display information. You can modify the script or add more stages as needed for a real-world scenario.

Feel free to customize the pipeline script according to your specific requirements. For any issues or improvements, refer to the [Issues](../../issues) section or create a pull request.
