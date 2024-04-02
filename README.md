1. Create a folder with name of the project
mkdir new-project
2. Go to the folder
cd new-project
3. Create Git repository
git init
4. Create a new file called README.md and add the some test to it
vim README.md
Save changes and exit from editor
5. Prepare the README.md  file for the commit
git add README.md
6. Commit the changes to the repository with commin message "Init"
git commit -m "Init"
7. Create a new branch called"development" and dwitch to it
git checkout -b development
8. Add the instructions to the README.md file and prepare them for the commit
vim README.md
Save changes and exit from editor
git add README.md
9. Commit changes to the "development" branch with a commit message
git commit -m "The instructions for creating the repository have been prepared"
10. Merge chamges from the "development" branch into the "main" branch
git checkout main
git merge development
11. Check the status, make sure everything is up to date.
git status
cat README.md
12. Commit changes to remote repository
git remote add origin https://<token>github.com/<username>/new-project
git push origin main
