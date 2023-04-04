# CoralApi
Backend API for Atelier

## GitHub workflow

### pull from group github main branch to local machine<br />
git checkout main<br />
git fetch origin <br />
git reset --hard origin/main<br />

### pull a branch that does not yet exist on your machine<br />
git fetch origin [branchName]:[branchName]

### create a new branch<br />
git checkout -b <branch_name>

### push the new branch to the group github.<br />
git push -u origin <branch_name>

### create a pull request to merge to "main" branch<br />
we do it on github

## to update your feature branch with up-to-date main
// Current branch : feature1 <br />
git switch main <br />
git pull origin main <br />
<br />
//now main branch in your local machine is up to date<br />
git switch feature 1<br />
git merge main<br />

// resolve conflict if any<br />
// commit changes

## useful log commands
// condense commit logs to a a single line list, includes full commit has
git log --pretty=oneline
![one line log example](https://user-images.githubusercontent.com/24556536/229687669-832d3e28-1d47-45df-a20c-bd5431d6d242.png)


// create a color coded visual graph with date, short commit hash, messages, and user (recommended to set as alias)
git config --global alias.hist "log --pretty=format:'%C(yellow)[%ad]%C(reset) %C(green)[%h]%C(reset) | %C(red)%s %C(bold blue){{%an}}%C(reset) %C(yellow)%d%C(reset)' --graph --date=short"
![customized graphic log example](https://user-images.githubusercontent.com/24556536/229687297-a79812cc-2301-40db-85ad-ac6e614107cf.png)
