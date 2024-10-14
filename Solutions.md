# Shell Exercises

## Exercise 1

- To navigate to the home directory, use `cd ~` or `cd`
- List all files with `ls`
- Navigate to any directory using `cd any-directory`
- To list files by time accessed, use `ls -t`
- File/folder accessed most recently will depend on person
- Navigate back to home directory
    - Relative path: `cd ../` or `cd ..`
    - Absolute path: `cd ~/`

## Exercise 2

- Create an empty file using `touch shrek.csv`
- Rename can be done using `mv shrek.csv donkey.csv`
- Can also be done using the `rename` function, but this will be more complicated.
    - `rename` is typically reserved for renaming many files/folders at once, thus the syntax is `rename 's/shrek.csv/donkey.csv/' shrek.csv`
- `mv` is used because we commonly rename files after moving them to a different directory.
- Delete the file using `rm donkey.csv`
    - **NOTE** `rm` is irreversible! Thus, this should be exercised with caution.

## Exercise 3

- Create an empty directory using `mkdir MammaMia`
- Create four text files using `touch file1.txt file2.txt file3.txt file4.txt`
- Move the text files using the `*` wildcard, which is a placeholder that matches any sequence of characters in a file name `mv *.txt MammaMia`
- Delete the directory using `rm -r MammaMia`
- Deleting a file requires no flag or option, while removing a folder which is not empty requires the `-r` option.
    - `rm -r` does recursive deletion, so it loops across all files inside the folder to delete everything

# Git and GitHub Exercises
## Exercise 1

- To create a folder in your home directory, first navigate to the home directory using `cd ~`.
- Next, create a folder using `mkdir my-first-repo`.
- Also create a folder using `mkdir git-repos`.
- Move the 'my-first-repo' folder into 'git-repos' using `mv my-first-repo git-repos/`. Navigate into 'git-repos/my-first-repo'.
- Make the folder a git repository using `git init .`.
- Create a README file using `touch README.md`.
- Use `git add README.md` to add the README to the staged files.
- Use `git commit -m "initial commit"` to make your first commit.
- Go to the GitHub home page (assuming you are logged in). The press on 'New' in the top-left corner.
- Enter the repository name ('my-first-repo') and description and **change the repository from public to private**.
- Press 'Create repository' on the bottom.
- Use the given commands to copy your 'my-first-repo' repository to GitHub.
    - This will be under "…or push an existing repository from the command line"
- Refresh the GitHub repository page.

## Exercise 2

- To make someone a collaborator, go to the repository website, click on 'Settings', then click on 'Collaborators' on the left-hand-side. Press 'Add people' and invite your team mate.
- To clone the repository, go to the repository's website, click on clone, copy the link, and then run `git clone [link here]` in your 'git-repos' folder. 
- To retrieve the current version of the repository, use 'git pull'.
- Create the file using 'touch [name-student].md' and open it using `open [name-student].md`. Edit the file in the opened text editor.
- Add the changes to the staged files using `git add [name-student].md`.
- Check the status using `git status`. Your file should now be staged.
- Use `git pull` to pull the current version.
- Use `git commit -m "[some message]` to commit the changes.
- Use `git push` to push the changes to the remote.

## Exercise 3

- Pull the repository using `git pull`.
- Use `mkdir about-students` to create the folder.
- Use `mv [student files] about-students/` to move all student files into the 'about-students' folder. Replace [student files] with the names of the student files separated by a space.
- Use `git add -A` to add all changes.
- Use `git commit -m [message]` to commit changes. Replace [message] with some informative message.
- Use `git push` to push to the remote.
- To edit the README, use `open README`.
- Add, commit, and push the changes as above.

## Exercise 4

- Pull the repo using `git pull`.
- Do the copying in any text editor. You can open the files from the shell using `open`.
- Add, commit, and push the changes like always.
- The team mate that gets a problem needs to use `git pull --rebase` first to pull the changes of the other team mate into their own README file.
- This will cause a merge conflict since both team mates worked on the same file and same lines.
- Can verify this happens by doing `git status`
- To solve this merge conflict, open the README in a text editor using `open` and make all the changes necessary.
- When ready, use `git add README` to add the README to the staged files.
- Continue the rebase using `git rebase --continue`.
- Then add, commit, push the changes to the remote like always.

## Exercise 5

- Pull the repo using `git pull`.
- Create a new branch using `git branch [student name]`.
- Move into the new branch using `git checkout [student name]`.
    - Can do both with one command by doing `git checkout -b [student name]`
- Create the new file using `touch [student-name]-research-interest.md`.
- Open the file using `open` and write about your interests.
- Add the changes using `git add .` and commit them using `git commit -m "[some message]"`.
- To push to the remote, use `git push -u origin [branch name]`.
    - This is the shorthand flag for `git push --set-upstream origin [branch name]`
- To create the pull request, go to the GitHub page, click on "Pull requests" at the top. Next, click on 'New pull request'. Set base to 'main' and set compare to the branch you created. Then press 'Create pull request'. Add a description and press 'Create pull request'.
- Merge the pull requests by clicking on 'Merge pull request'. Delete the branch afterwards on GitHub.
- Back in the shell, run `git checkout main` to go back to the main branch.
- Run `git branch --delete [student name]` to delete the branch you created.

## Exercise 6

- Create the new branch as in Exercise 5.
- Commit the changes to the remote branch as in Exercise 5.
- Create the pull request as in Exercise 5.
- Merge one of the pull requests as in Exercise 5.
- You will not be able to merge the second pull request, because the changes that you and your team mate made are conflicting. To resolve this, the student with the conflicting pull request needs to go back to the shell.
- In the shell, go to the main branch using `git checkout main`.
- Get the current version of main by running `git pull`.
- Then go back to the other branch using `git checkout [student name]`.
- Run `git merge main` to merge the changes of main into the current branch. You will get a merge conflict warning.
- Open README.md in a text editor. You should now see the common merge conflict. Fix the conflict in the text editor.
- Add, commit, and push the README changes to remote using `git add README.md`, `git commit -m "[some message]"`, and `git push`.
- Go back to the pull request and refresh the page. You should now be able to merge the pull request.
