This guide will walk you through creating a repository on GitHub, connecting it to your local machine, making changes to your project, and finally pushing those changes to your online repository.

Requirements:

A GitHub account (Sign up for free at https://github.com/join)
Git installed on your local machine (Installation instructions can be found at https://git-scm.com/downloads)
A code editor of your choice e.g., Visual Studio Code

Step 1: Creating a Repository on GitHub

Log in to your GitHub account and click on the "New repository" button.
In the "Name" field, enter a descriptive name for your project. We'll use "PLPBasicGitAssignment".

Under "Initialize this repository with a README", select the option to create a README file. A README is a text file typically found in the root directory of a project that provides information and instructions. We'll create a more detailed README later, but for now, having a basic one is helpful.
Click on the "Create repository" button to finalize your repository creation on GitHub.

Step 2: Setting Up Your Local Project

Open a file explorer window on your computer and create a new folder. Name it the same as your GitHub repository, in this case "PLPBasicGitAssignment".

Now, open a terminal window or command prompt,or gitbash if already installed. You can usually find this application by searching for "terminal" or "command prompt" in your start menu.

Use the cd command to navigate to your newly created folder. For example, if your folder is on your desktop, you might type:
cd Desktop/PLPBasicGitAssignment

Once you're in the correct directory, type the following command to initialize a new Git repository in your local folder:
git init
This creates a hidden folder named ".git" in your local directory. This folder stores important Git data about your project.

Step 3: Connecting Your Local Project to GitHub

To link your local repository to your online repository on GitHub, you'll use the git remote add command in your terminal window. This command tells Git where to push your local commits.
git remote add origin <repository-url>

Replace <repository-url> with the actual URL of your GitHub repository. You can find this URL by going to your repository on GitHub and copying the address from the web browser. It will look something like https://github.com/<your-username>/PLPBasicGitAssignment.git.

Step 4: Making Changes and Committing Them

Now that everything is connected, let's create a new file to demonstrate how Git tracks changes. Open your preferred code editor and create a new text file inside your local "PLPBasicGitAssignment" folder. Name the file "hello.txt".

In your code editor, add a line of text to your "hello.txt" file, such as "Hello, Git!". Save the changes to the file.

Back in your terminal window, use Git commands to record (or "commit") the changes you made to the file.

First, use the git add command to tell Git which files you want to include in your next commit:
Bash
git add hello.txt
This stages the changes you made to "hello.txt" for the next commit.

Next, use the git commit command to create a snapshot of the current state of your project with a descriptive message:
git commit -m "message"
Replace the message in quotes with a brief description of your changes. This message helps you and others understand what changes were made in this commit.

Step 5: Pushing Your Changes to GitHub
Finally, use the git push command to upload your committed changes to your GitHub repository:
git push -u origin main
This command pushes your local commits to the "main" branch of your remote repository on GitHub.

The -u flag is a shortcut that sets the upstream branch for your local "main" branch. You'll only need to use this flag the first time you push to your remote repository.

