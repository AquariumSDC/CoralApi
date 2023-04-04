# CoralApi
Backend API for Atelier

GitHub workflow
pull from group github main branch to local machine
git checkout main
git fetch origin
git reset --hard origin/main

pull a branch that does not yet exist on your machine
git fetch origin [branchName]:[branchName]

create a new branch
git checkout -b <branch_name>

push the new branch to the group github.
git push -u origin <branch_name>

create a pull request to merge to "main" branch
we do it on github

to update your feature branch with up-to-date main
// Current branch : feature1
git switch main
git pull origin main

//now main branch in your local machine is up to date
git switch feature 1
git merge main

// resolve conflict if any
// commit changes
