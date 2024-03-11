GIT ASSIGNMENT
LOGESHWARAN A

Question 1
Step 1: Create a new Git repository.
Ans: Created new repository in git hub.
Command in Git or In PyCharm Terminal : mkdir “folder_name”
Step 2: Create a file and commit changes.
Ans: git add ., git commit -m “commit_message”, git push origin main  
Step 3: View the commit history of your repository.
Step 4: Open the file you created earlier and make some changes to it. 
Ans:  make some changes in file
Step 5: Check the file you modified is now marked as "modified" and unstaged. 
Hint (git status)
Step 6: Stage the changes you made to the file and commit the changes to the repository.
Ans: git add ., git commit -m “commit_message”, git push origin main  - Commands to commit the changes.
Step 7: Clone the repository you have created in GitHub.
Ans: commands – git clone “Repo_Link”
Step 8: Fetch the changes, navigate into the cloned repository using the command line, and use the command git fetch to fetch any changes that have been made to the original repository since you cloned it.
Ans: Commands – git fetch (fetch the changes from github), git merge (commit the changes)
Step 9: Pull changes, merge the changes you just fetched into your local copy of the repository, and use the command git pull.
Ans: git pull (commit the changes in the GitHub to local Repo), git merge (commit the changes form one branch to another branch)

Question 2
Step 1: Clone the repository you have created in GitHub.
Ans: commands – git clone “Repo_Link”
Step 2: Create a new branch using the command.
Ans: Command – git branch “Branch_name”
Step 3: Switch to the new branch.
Ans: Command – git checkout “new_branch”
Step 4: Make some changes to the code in your local copy of the repository.
Ans: make any changes in file or create a new file
Step 5: Commit changes to the new branch.
Ans: git add ., git commit -m “commit_message”, git push origin new_branch 
Step 6: Switch back to the original branch
Ans: git checkout main
Step 7: Merge the new branch.
Ans: git merge new_branch
Step 8: Push changes to the original branch
Ans: git add ., git commit -m “commit_message”, git push origin main

Question 3
Step 1: Create a feature branch. Ans: git branch new_branch
Step 2: Switch to the new branch. Ans: git checkout new_branch
Step 3: open the file and make some changes to it.
Ans: Create new file and add changes
Step 4: Add and commit the changes to the new branch.
Ans:  commit changes using - git add ., git commit -m “commit_message”
Step 5: Push the changes to the new feature branch.
Ans: git push origin “new_branch”
Step 6: Create a pull request.
Step 6: As another user in the master branch make some changes to the same file.
Ans: Make any changes in the master branch with the same file. And commit changes
Step 7: Add and commit the changes to the master branch.
Ans: git add ., git commit -m “commit_message”
Step 8: Push the changes to the master branch. Ans: push the changes using merge
Note: There will be a conflict in the pull request, how do we resolve it??
Ans: If there is any changes in the same file and if we try to merge the branches it will show conflict. To resolve conflict we used to change the modification in the file and try to merge the conflict changes using rebase, 
Hint: git rebase

Question 4
Step 1: Step 1: Create a feature branch.
Step 2: Switch to the new branch.
		open the file and make some changes to it.
		Add and commit the changes to the new branch.
		open the same file and make some changes to it.
		Add and commit the changes to the new branch.
		open the same file and make some changes to it.
		Add and commit the changes to the new branch.
Step 3: Identify the commit or commits that you want to "cherry-pick"(Note the hash of the commit or commits that you want to "cherry-pick")
Ans: git log - -oneline (This command gives the commits made in oneline with commit Id
Step 4: Use the "git checkout" command to switch to the branch where you want to apply the changes.
Ans: git checkout main_branch
Step 5: Use the "git cherry-pick" command followed by the commit hash(es) that you want to apply.
Ans: git cherry-pick “commit_id”
It is used to commit the specific changes 

Question 5
Step 1: Step 1: Create a feature branch.
Ans: git branch “new_branch”
Step 2: Switch to the new branch.
		open the file and make some changes to it.
		Add and commit the changes to the new branch.
		open the same file and make some changes to it.
		Add and commit the changes to the new branch.
		open the same file and make some changes to it.
		Add and commit the changes to the new branch.
Step 3: Use the "git log" command to view the commit history and identify the commit to which you want to reset.
Step 4: Use the "git reset" command followed by the desired reset type and the commit hash
Step 5: Verify that the reset was successful by using the "git log" command again. 
Ans: git log –oneline (gives the changed commits)
Step 6: Use the "git log" command to view the commit history and identify the commit that you want to reverse.
Ans: git log –oneline (gives the changed commits)
Step 7: Use the "git revert" command followed by the commit hash or reference to which you want to revert. (Hint: git revert <commit hash>)
Step 8: Verify that the revert was successful by using the "git log" command again. 
Ans:git log --oneline (This command gives the commits we have done in one line with commit I'd or hash)
Note: Identify the difference between git log after git reset and git revert.
Ans: After using git reset, the commits that were removed from the branch's history will not appear in git log unless you explicitly reference them using a commit hash or a different branch. After using git revert, the reverted commits remain in the history, and you can see them in git log along with the new commit(s) created by the revert operation. These new revert commits will appear in the history alongside the original commits.

