# Continuous Collaboration Workflow

Assuming you are working on a market feature on FormFolio

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
Repeat this for both the backend and frontend repositoris.
Reach out to the team incase of any challenges.
