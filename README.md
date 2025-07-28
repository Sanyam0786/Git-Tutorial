# Git-Tutorial

Name : Sanyam Mujavadia

* **Initialize a New Local Repository** : `git init`

* **Git Clone** : `git clone <Repository Url>`

* **Git Pull** : `git pull origin main`

* **Git Push** : `git push origin main`

* **Git Add** : `git add <file-name>` (If there is multiple file to add then insted of using "file-name" one by one you can us "." to access all file at once)

* **Git Commit** : `git commit -m "Message"`

* **View Commit History** : `git log`

* **Git Create new branch** : `git branch <New-branch-name>` 

* **Git Create and switch to a new branch** : `git checkout -b <New-branch-name>`

* **Git Branch Merge** : `git merge <branch-name>`

* **Git Branch Creation** : `git branch <branch-name>`

* **Git Stashing** : `git stash` (Save unfinished work temporarily, to come back later),
`git stash pop` (Restore stashed changes)
`git stash push -- <file-name>` (For Stashing a specific file)
`git stash push -m "Message" -- <file-name>` (Adding message in the stash file)

* **Git Revert** : `git revert <commit-hash>` (Creates a new commit that reverses a previous commit) (Better to use if the commit is push in the repo)

* **Git Reset** : `git reset <commit-hash>` (Moves branch pointer to a specific commit, deleting commits after that) (Better to use if the commit is not push in the repo)

* **Git Fork** : Go to the repo which you wanna fork and then there is a button called "Fork" in the repo that create a copy repo in your own account and you can contribute your changes to the main repo by sending pull request to the main account branch and if the user found your changes usefull they will accept the pull request or just give some comment on your pull request. 

* **Git Restore** : `git restore <file-name>` (It discards unstaged changes in your working files and reverts them to the last committed version),
`git restore --staged <file-name>` (Unstage a file and keep changes in working directory),
`git restore --source <commit-hash> <file-name>` (Restore a file to how it was <commit-hash> ago)

<-------------------------------------------------------------------------------------------------->

# <-- Workflow (Repo already created in the account) -->

1.  **Clone the Repository** - Get a local copy of the project:
    ```bash
    git clone <repository-url>
    ```

2.  **Move into the Repository Directory** - Navigate to your project folder:
    ```bash
    cd project
    ```

3.  **Create a Branch for a New Feature** - Work on new features or fixes in an isolated branch:
    ```bash
    git checkout -b branch-name
    ```

4.  **Make Changes, Stage, and Commit** - After making your code changes, prepare and save them:
    ```bash
    git add .
    git commit -m "Message"
    ```

5.  **Push Your Branch to the Remote** - Share your new branch and its commits with the remote repository:
    ```bash
    git push origin branch-name
    ```

6.  **Merge the Branch (After Review)** - Once your changes are reviewed (e.g., via a Pull Request), integrate them into the `main` branch:
    ```bash
    git checkout main
    git merge branch-name
    ```
    *(Note: Ensure you replace `branch-name` with the actual name of your feature branch.)*

7.  **Pull the Latest Changes from Remote** - Keep your local `main` branch synchronized with the remote:
    ```bash
    git pull origin main
    ```