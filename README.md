Exercise Day 3 

Steps

1. Clone this repository on your computer. If you have already cloned the repository, go to the folder where the repository is.
2. Go to the master branch and get the last changes on the repository. [git checkout master; git pull]
3. Create a new branch. (example: solve_exercise_valentina) [git branch <branch name>]
4. Checkout to the newly created branch. [git checkout <branch name>]
5. See what commit created the file with your name. [git blame your_name.txt]
6. Copy the id of the commit.
7. Revert the commit [git revert <commit_id>]
8. Check the difference between your branch and master. This should show you what animal was in that file before, if you forgot it. [git diff master]
9. Write the animal into "animale.txt" and save the file.
10. Add the file "animale.txt" into the staging area, then commit. [git status, git add "animale.txt", git commit -m "..."]
11. Publish your branch to the remote repository. [git push --set-upstream origin <branch_name>]
12. Create a pull request to merge your branch into master. Check the differences before creating the pull request to make sure you have not done anything wrong! (this can be done from github)
13. Take care of yout pull request and make sure there are no conflicts! If there are no conflicts, merge your branch and you are done! :D
  
  
**If you have conflicts:**
1. Go to the master branch and get the last changes on the repository. [git checkout master; git pull]
2. Go back to your branch. [git checkout <branch name>]
3. Merge the branch master into your branch. This will bring all the new changes into your branch and this will allow you to solve the conflicts in your branch, without breaking the master branch. [git merge master]
4. The previous step will show that you have conflicts. If you run "git status", you will see the conflicted file marked with "Both modified:"
5. Open the conflicted file. Solve the conflicts! Make sure to check the difference and correct the errors BEFORE removing the "======" parts. Removing the "======" parts should be the last step. Save the changes.
6. Add the conflicted file with "git add <filename> and commit [git commit]
7. Push to remote repository [git push]
8. Go to the pull request page, refresh and check to see if you can merge now! If there are no conflicts, merge your branch and you are done! :D
