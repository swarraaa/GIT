# Repository:

- A Git repository is a data structure that stores a collection of files, along with the history of changes made to those files over time.
- It is commonly used for version control, allowing multiple people to collaborate on a project, track changes, and manage different versions of the files.
- It can contain folders, files, images, videos, spreadsheets, datasets- anything a project needs!
- Types: 1.Local 2.Remote

# Architechture:

## Three Tree Architechture:

<div align="center">
<img src="https://res.cloudinary.com/dduur8qoo/image/upload/v1685255623/GitArchitecture_wqhc9l.png" alt="three tree architecture of Git" height="200" float="right"/>
</div>

### The local repository has three virtual zones or areas viz. working area, staging area and commit area

1. <b>Working area:</b> This is where you make changes to your files, like creating new files, modifying existing ones, or deleting them
2. <b>Staging area (Index):</b> After making changes in the working area, you add them to the staging area. It acts as a holding area where you select specific changes or files to be included in the next commit.
3. <b>Commit area (Repository):</b> When you're ready to permanently save your changes, you create a commit. A commit captures a snapshot of your project with the changes from the staging area. It becomes part of the commit history in the repository.

# Workflow:

<div align="center">
<img src="https://res.cloudinary.com/dduur8qoo/image/upload/v1685255625/GitWorkflow_e8awyt.png" alt="three tree architecture of Git" height="400" float="right"/>
</div>

## Working:

1. First and foremost, there is no Git repository. To start working with Git, you need to create a Git repository using the command `git init`. This sets up the foundation for version control in your project.

2. Once the Git repository is initialized, you enter the working directory where you can freely make changes to your project. This includes creating new files, modifying existing ones, or deleting them. The files in this area are considered "untracked" by Git.

3. Once you are done, you can add all these changes or only the required ones to the staging area using the command `git add <filename>` or `git add .`. This will start tracking the changes, and the files will be "staged".

4. When you are satisfied with the changes in the staging area, you can create a commit to permanently save them with the command `git commit -m "Commit message"`. The files will then move to the commit area and be in the "unmodified" state.

5. If you want to make changes to a committed file, the files will be moved back to the working area and will be in the "modified" state. You can repeat the same procedure by adding and committing the changes to create different versions of the code.

6. Additionally, you can stop tracking files by using the `git rm <filename>` command. This removes the file from the working directory and stages its removal for the next commit.

## Actions:

1. Initialize a Repository: Create a new Git repository for your project using the command `git init`.

2. Add Files: Start by adding the necessary files to the repository using `git add <file>` or `git add .` to add all files.

3. Review Changes: Use `git status` to see the status of your files and the changes you've made.

4. Commit Changes: Once you're satisfied with your changes, create a commit with a descriptive message using `git commit -m "Commit message"`.

5. Repeat Steps 2-4: Continue modifying files, adding changes to the staging area, and committing as needed.

6. View Commit History: Use `git log` to see a history of commits, including their messages and unique identifiers.

7. Create Branches: Use branches to create separate lines of development. Start a new branch with `git branch <branch-name>` and switch to it using `git checkout <branch-name>`.

8. Merge Branches: Incorporate changes from one branch into another using `git merge <branch-name>`.

9. Handle Conflicts: If conflicts occur during a merge, resolve them manually by editing the conflicting files, then add and commit the changes.

10. Connect to Remote Repository: Connect your local repository to a remote repository using `git remote add origin <remote-url>`.

11. Push to Remote Repository: Upload your local commits to the remote repository using `git push origin <branch-name>`.

12. Pull from Remote Repository: Download the latest changes from the remote repository using `git pull origin <branch-name>`.

13. Clone a Repository: Create a local copy of a remote repository with `git clone <remote-url>`.
