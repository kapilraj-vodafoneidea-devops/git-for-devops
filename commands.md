 "git":
            echo "Related commands for Git:"
            echo "1. git status - Show the working tree status."
            echo "2. git add . - Add all changes to staging."
            echo "3. git commit -m 'message' - Commit changes with a message."
            echo "4. git branch -a - List all branches."
            echo "5. git checkout [branch] - Switch to another branch."
            Here’s a step-by-step guide to using Git, from setting up a repository to pushing changes to a remote repository like GitHub or GitLab.

Step-by-Step Git Workflow
1. Setup Git (One-time setup)
Configure your Git environment:

bash
Copy code
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
Verify the configuration:

bash
Copy code
git config --list
2. Initialize a Git Repository
Navigate to your project directory and initialize a new Git repository:

bash
Copy code
cd /path/to/your/project
git init
3. Add Files to the Repository
Add all the files in the project to the staging area:

bash
Copy code
git add .
To add a specific file, use:

bash
Copy code
git add filename
4. Check the Status
Before committing, check the current status of your files:

bash
Copy code
git status
This shows which files are staged for the next commit and which are not.

5. Commit Changes
Once you've staged the files, commit them to the repository with a message:

bash
Copy code
git commit -m "Your commit message"
6. Create a New Branch (Optional)
If you're working on a feature or bug fix, it's a good practice to create a new branch:

bash
Copy code
git branch feature-branch-name
git checkout feature-branch-name
Or use a single command to create and switch to the new branch:

bash
Copy code
git checkout -b feature-branch-name
7. Connect to a Remote Repository
If you’re working with a remote repository (e.g., GitHub or GitLab), add the repository URL:

bash
Copy code
git remote add origin https://github.com/username/repository.git
8. Push to Remote Repository
If it's the first push, you need to specify the branch explicitly:

bash
Copy code
git push -u origin master
For subsequent pushes, you can use:

bash
Copy code
git push
9. Pull Updates from Remote
To pull the latest changes from the remote repository to your local branch:

bash
Copy code
git pull
10. Merge Branches
Once your feature is ready, switch back to the main branch and merge the feature branch:

bash
Copy code
git checkout master
git merge feature-branch-name
11. Resolve Conflicts (If Any)
During the merge, you might encounter conflicts. Git will show you which files have conflicts. Open those files, resolve the conflicts, and then:

bash
Copy code
git add conflict-file
git commit -m "Resolved conflict"
12. Delete the Feature Branch
After merging, you can delete the feature branch:

bash
Copy code
git branch -d feature-branch-name
13. View the Commit Log
To view the history of commits in the repository:

bash
Copy code
git log
Summary of Common Git Commands:
Step	Command	Description
Setup	git config --global user.name "Your Name"	Set up Git name
Initialize	git init	Initialize a Git repository
Add files	git add .	Stage all files
Commit	git commit -m "Message"	Commit staged files
Branch	git checkout -b branch-name	Create and switch to new branch
Remote	git remote add origin <url>	Add remote repository URL
Push	git push	Push changes to remote
Pull	git pull	Pull changes from remote
Merge	git merge branch-name	Merge a branch into the current branch
Log	git log	View commit history
