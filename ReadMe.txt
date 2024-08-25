Git Commands and Workflow
Initialize a Git Repository:

git init
This initializes a new Git repository in your current directory.

Clone a Repository:

git clone <URL>
This clones an existing repository from a remote server to your local machine.

Create a New Branch:\

git branch <your branch name>
This creates a new branch from the current branch (often main or master).

Switch to the New Branch:

git checkout <your branch name>
This switches to the newly created branch.

Make Changes in Your Code: After making changes in your code (adding, modifying, or deleting files):

Stage Changes:

git add .
Adds all changes to the staging area.

git add <filename>
Adds specific files to the staging area.

Stash Changes (Optional):

git stash
Temporarily saves your changes and reverts the working directory to the last committed state. This is useful if you need to switch branches without committing your current work.

Commit Changes:

git commit -m "<your commit msg>"
Commits the staged changes with a descriptive message.

Push Changes to Your Branch:

git push origin <your branch name>
Pushes the committed changes to the remote repository in the specified branch.

Create a Merge Request:

After pushing your changes, you can create a merge request (or pull request) to have your changes reviewed and eventually merged into the main branch.

Additional Git Commands:
Pull Latest Changes:

git pull
Pulls the latest changes from the remote repository into your current branch, automatically merging them.

Fetch Latest Changes:

git fetch
Downloads the latest changes from the remote repository but does not merge them. It keeps the changes in a separate history until you merge them manually.

Cherry-Pick Specific Commits:

git cherry-pick <hashcode>
Applies a specific commit from another branch to your current branch.

Squash Commits:

git rebase -i HEAD~<n>
This is the correct way to squash multiple commits into one. During an interactive rebase, you can choose to squash (s) multiple commits into a single commit.

git rebase -i HEAD~3
This opens an editor where you can choose to squash the last three commits.
Note: Squashing is not a standalone command but part of an interactive rebase. It’s useful for cleaning up a commit history before merging.