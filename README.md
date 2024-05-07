# Continuous Collaboration Workflow

Assuming you are working on the Market feature on FarmFolio. You will have to follow this steps for both the frontend and backend.. You dont have to fork the repository. Thats optional.

The backend clone link:  git@github.com:NB-Kamoni/FarmFolio-Backend.git

The frontend clone link: git@github.com:KelvinMugo4500/farm-folio.git

## Clone the Repository


```
git clone <repository-url>
cd <repository-name>
```


## Add upstream remote

```
git remote add upstream <original-repository-url>
```


## Create a new branch
You can use prefixes for branch names: FT- for featuture, BG- for bug fix.. eg FT-Market.

```
git checkout -b <branch-name>
```


## Code and make changes
## Stage and commit changes

```
git add .
git commit -m "Your commit message"

```

## Push changes to your branch

```
git push origin <branch-name>
```

## Create a pull request
Go to the original repository on GitHub.
Switch to the branch you just pushed (your branch).
Create a pull request with your changes.
Select Kelvin as the reviewer

You are done  :)

## Kelvin Reviewer/Tester

He will review the PRs and merge to main branch

```
git fetch upstream
git checkout main
git merge upstream/main
git push origin main
```


## What next? Getting updated work to your local

After Kelvin does the merging, each team member should update their clones so that they can also work with what was merged. 

To get the latest changes from your remote repository, fetch the updates. This won't change your local files but will update the remote tracking branches:

```
git fetch origin

```

Now, check if your branch has diverged from the remote branch or if there are new changes:

```
git status

```

To update your branch with the latest changes from the remote repository, use git pull. This will fetch and merge the changes from the remote branch into your current branch:

```
git pull origin <current branch>

```

If there are conflicts when you pull, you'll need to resolve them before you can proceed:

Git will point out where the conflicts are.
Edit the conflicting files to resolve the conflicts.
Use git add <file> to mark the conflict as resolved.
Commit the resolution with git commit.


## You are done!

confurm that you have the updates 

```
git status

```

Repeat this for both the backend and frontend repositoris.
Reach out to the team incase of any challenges.

