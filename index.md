Assignment 1.5 — GitHub Essentials II
Objective: Upload a local project to GitHub, create two commits, and verify the commit history.
Step 1: Create a GitHub account
1. Open GitHub.
2. Sign up for a new account or log in to your existing account.
Step 2: Create a public repository
1. Click the + icon in the top-right corner and select New repository.
2. Enter the repository name: web-development-practice
3. Select Public.
4. Leave “Add a README file” unchecked if your local project already has files.
5. Click Create repository.
Keep the repository page open because you will need its URL.
Step 3: Connect your local project to GitHub
Open the terminal in VS Code inside your project folder.

First, check whether Git is initialized:
git status


If it says the directory is not a Git repository, run:
git init


Configure your Git username and email (use your own details):
git config --global user.name "Your Name"
git config --global user.email "your-email@example.com"


Stage and commit your project files:
git add .
git commit -m "Initial commit"


Rename the branch to main:
git branch -M main


Connect your local repository to GitHub. Replace the URL with your actual repository URL:
git remote add origin https://github.com/YOUR-USERNAME/web-development-practice.git


If origin is already configured, check it with git remote -v instead of adding it again.
Step 4: Upload files using git push
Run:
git push -u origin main


If prompted, complete GitHub authentication in your browser.

After the command succeeds, refresh your GitHub repository page. Your project files should appear there.
Step 5: Add a new file and push the second commit
Create a new file named assignment-1.5.md in your project folder.

Add the following content:
Assignment 1.5 — GitHub Essentials II
Objective
Upload a local project to GitHub and verify the commit history.
Tasks Completed
- Created or accessed a GitHub account.
- Created a public repository.
- Connected the local repository to GitHub.
- Uploaded project files using git push.
- Added a new file and created a second commit.
- Verified the commit history on GitHub.




Save the file, then run these commands in the terminal:
git add assignment-1.5.md
git commit -m "Add Assignment 1.5 documentation"
git push


You have now created the second commit and uploaded it to GitHub.
Step 6: Verify the commit history
Run this command in VS Code:
git log --oneline


You should see two commits similar to these:
a1b2c3d Add Assignment 1.5 documentation
e4f5g6h Initial commit


The letters and numbers will differ on your computer.

Finally, open your GitHub repository and click Commits to verify that both commits appear online.

Submission
Submit the link to your public GitHub repository in this format:

https://github.com/YOUR-USERNAME/web-development-practice

Replace YOUR-USERNAME with your actual GitHub username.

Important: Submit the real repository link only after successfully pushing your files and verifying the commit history.