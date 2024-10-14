> [!NOTE]
> You are only allowed to use the shell, a text editor, and a internet browser for all exercises. The internet browser is only allowed for the GitHub related pull requests. All other tasks can and should be done in the shell and a text editor.

- Students should form teams of two
- In these teams, work on the exercises
- We always discuss an exercise together before moving on to the next, unless a team is really fast and is getting bored

# Shell Exercises

## Exercise 1

- Navigate to your home directory
- List all files in your home directory
- Navigate to a subdirectory within your home directory
- List all files and directories in the subdirectory by time accessed
- Which file/folder was accessed most recently?
- Navigate back to the home directory using relative paths

## Exercise 2

- While in the home directory, create an empty file called 'shrek.csv'
- Rename that file to 'donkey.csv'
- Delete 'donkey.csv'

## Exercise 3

- While in the home directory, create an empty directory called 'MammaMia'
- Create four text files, named anything you like, with one command in the current directory
- Move all four text files into the 'MammaMia' directory with one line of code
- Delete the directory 'MammaMia'. What is the difference in deleting a file and deleting a folder?

# Git and GitHub Exercises

## Exercise 1

- Create a folder in your home directory. Call it 'my-first-repo'.
- Create a directory in your home directory called 'git-repos'.
- Move 'my-first-repo' into the 'git-repos' directory.
- Make the 'my-first-repo' a git repository.
- Create a README file.
- Upload the repository to GitHub (make it a private repository).

> [!NOTE]
> Typing a password into the CLI will not make it visible, but rest assured, the password is being typed.
> Additionally, including your password into the CLI may cause problems. This simply means you have to create a personal access token. Read [here](https://stackoverflow.com/questions/68775869/message-support-for-password-authentication-was-removed) for how to set this up.
> If you plan on using Git for extended periods of time, it is wise to instead set up SSH. We won't go into this, but instructions to set it up can be found [here](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account).

## Exercise 2

- Make both team mates a collaborator for the 'my-first-repo' repository created in Exercise 1.
- Each team mate: Clone the repository.
- Each team mate: retrieve the current version of the repo using `pull`.
- Each team mate: Create a `[name-student].md` file in the repository and write a paragraph about yourself.
- One after another: Commit the changes and push them to the remote repository. Pull before you push!

## Exercise 3

- First team mate: pull the repository.
- First team mate: Move all `name-student.md` files into a folder titled 'about-students'.
- First team mate: Push the new changes to the remote.
- One team mate: Edit the README.md. The title should be the name of your team (come up with something creative).
- Create a second header underneath (new section) titled "About".
- Push changes to remote.

## Exercise 4
- Each team mate: pull the repo.
- Each team mate: copy your about text from the `[name-student].md` file into the README file under the 'About' section.
- Each team mate: Push the changes to the remote.
- One of the team mates will likely get a *merge conflict*. Use the reading material to resolve the merge conflict together.

## Exercise 5

- Each team mate: pull the repo.
- Each team mate: create a new branch with your name as name.
- Each team mate: enter the new branch.
- Each team mate: create a new file entitled '[student-name]-research-interest.md'.
- Each team mate: write one or two paragraphs about your research interest.
- Each team mate: push the new branch to the remote.
- Each team mate: create a pull request to merge the branch into the main branch.
- One team mate: merge all pull requests.
- Each team mate: switch back to the main branch and delete the branch you created.

## Exercise 6

- Each team mate: create a new branch with your last name as a name.
- Each team mate: enter the new branch.
- Each team mate: edit the README.md. Add some information about your hobbies under the text you wrote before.
- Each team mate: commit the changes and push them to the remote branch.
- Each team mate: create a pull request to merge your new branch into main.
- One team mate: merge one of the pull requests.
- One team mate: try to merge the other pull request. This should not be possible.
- One team mate: fix the problem.


# Preparation for DSRI

# Exercise 1

> [!WARNING]
> If you are  too slow, this might crash some computers. Please save all important work before you do this exercise.

- Use the following (intentionally slow) implementation of Fibonacci numbers to find the first 1 million numbers.
```r
fib_slow <- function(n) {
  if (n==1) return(1)
  if (n==0) return(0)
  return(fib_slow(n-1) + fib_slow(n-2))
}
lapply(1:1e6, fib_slow)
```
- Open your shell.
- Download a process viewer such as top, htop, or bottom
- Find the R process in a process viewer (in the shell, do not use any GUI).
- How much RAM is the process using? Is it increasing over time?
- How much CPU is the process using? What process is currently using the most CPU?
- Kill the R process before it kills your computer.
