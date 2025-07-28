# Git-Tutorial

Name : Sanyam Mujavadia

Git Clone : git clone <Repository Url>

Git Pull : git pull origin main

Git Push : git push origin main

Git Commit : git commit -m "Message"

Git Branch Merge : git merge <branch-name>

Branch Creation : git branch <branch-name>

Git Stashing : git stash

Git Revert : git revert <commit-hash>

Git Reset : git reset <commit-hash>


# Workflow

# 1. Clone the repository
git clone <repository-url>

# 2. Move into the repository
cd project

# 3. Create a branch for a new feature
git checkout -b branch-name

# 4. Make changes, then stage and commit
git add .
git commit -m "Message"

# 5. Push your branch to the remote
git push origin branch-name

# 6. Merge the branch once reviewed
git checkout main
git merge branch-name(different from current checkout branch)

# 7. Pull the latest changes from remote
git pull origin main
