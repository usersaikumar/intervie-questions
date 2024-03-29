# GIT
- Source Code Management
- Version Control System
- De-Centralized

## Branching Strategy
- Feature Branch
- Release Branch
- Git Flow
- GiHub Flow

### Feature Branching
- This branching type ensures that a particular feature of a project is maintained in a branch.
- Once the feature is fully validated, the branch is then merged into the main branch.
### GitHub Flow
- Creating a Branch
  - Branches help you work on features, Fix bugs
  - Do not effect master branch
  - Anything in the master branch is deployable
- Add Commits
  - Keeps track of changes in your feature branch
  - More transparent history of work
  - A separate unit of change
- Open a Pull Request
  - Discussion about your commits
  - Open it during any point of your development process
  - You can ask feedback from any of your team members
  - Pull request frame a problem by describing it
  - Reviewer is aware of your problem statement
  - A basic run through from setup to expected outcome is recommended
- Discuss and Review your Code
  - People reviewing your code might have feedback
  - A review focusses on the code health and on production readiness
  - Code health & Production Readiness
- Test Your Changes
  - Test in a production like Environment
  - Update your tool
- Merge your Feature
  - Finally merge your Code
  - Pull Requests preserve a record of the histroical changes to your code

## Git Pull
- git pull is a Git command used to update the local version of a repository from a remote.
- git pull fetches (git fetch) the new commits and merges (git merge) these into your local branch.
```
git pull origin
```
## Git Pull Request

- A pull request is an event in Git where a contributor asks a maintainer of a Git repository to review code they want to merge into a project.
- The process for a pull request approval in Git will involve getting the project maintainer(s) to review your work; after which they will provide comments or, if your pull request is approved, will merge your changes directly into the main repository. 

```
pull request in git hub have to review and accept
```
## Git Fetch

- git fetch is the command that tells your local git to retrieve the latest meta-data info from the original (yet doesn’t do any file transferring. It’s more like just checking to see if there are any changes available).

```
git fetch origin
```
## Git Merge
- The git merge command lets you take the independent lines of development created by git branch and integrate them into a single branch.
- you have to create a branch and done your changes and checkout to main and merge your branch
1. Merge
2. Fast Farward Merge (likely Rebase)
3. 3-way Merge
```
git merge branch_Name
```
## Git Rebase

- Rebasing is the process of moving or combining a sequence of commits to a new base commit. Rebasing is most useful and easily visualized in the context of a feature branching workflow.
- it is following sequence of commits
```
git rebase origin
```
## Git Revert

- The git revert command is a forward-moving undo operation that offers a safe method of undoing changes.
```
git revert HEAD~1 (or) [commit_id]
```
## Git Reset

- The git reset command is a complex and versatile tool for undoing changes. It has three primary forms of invocation. These forms correspond to command line arguments --soft, --mixed, --hard.
- git reset == undo to working irectory
- --soft == undo to staging area
- --hard == delete whole file
```
git reset Head~1 (or) commit_id
git reset --soft Head~1 (or) commit_id
git reset --hard Head~1 (or) commit_id
git reset --mixed Head~1 (or) commit_id
```
## Git Stash
- Git stash is a built-in command 
- that locally stores all the most recent changes in a workspace and 
- resets the state of the workspace to the prior commit state.
- we can create branch from stash also
```
git stash
git stash list
git stash clear
git stash show -p stash{ }
git stash branch branch_name stash{ }

```

## Git Stash Apply and Git Stash Pop
- You can reapply previously stashed changes with git stash pop:
- Alternatively, you can reapply the changes to your working copy and keep them in your stash with git stash apply:
- Adding the -u option (or --include-untracked) tells git stash to also stash your untracked files:

```
git stash pop stash{ }
git stash apply stash { }
```

## Git Stash drop
- If you decide you no longer need a particular stash, you can delete it with git stash drop:

```
git stash drop stash { }
```
## Git Cherrypick
- git cherry-pick is a powerful command
- Cherry picking is the act of picking a commit from a branch and applying it to another. 
- git cherry-pick can be useful for undoing changes. 
- For example, say a commit is accidently made to the wrong branch. You can switch to the correct branch and cherry-pick the commit to where it should belong.
- ```git cherry-pick commit_id```
## Git diff
- Comparing changes with git diff
- By default git diff will show you any uncommitted changes since the last commit.
- Comparing files between two different commits
- Comparing two branches

```
git diff
git diff commit_id commit_id
git diff branch_name1..branch_name2
```
## Git status
- The git status command is a relatively straightforward command. It simply shows you what's been going on with git add and git commit.

```
git status
```
## Git Log
- The git log command displays committed snapshots.

```
git log
git log -n 2
git log --oneline
git log <since>..<until>
git log <file>
```
## Git Remote
- The git remote command lets you create, view, and delete connections to other repositories. 
- Viewing git remote configurations 
- ```git remote``` ```git remote -v```
- Creating and modifying git remote configurations 
- ```git remote add <name> <url>``` 
- ```git remote rm <name>``` 
- ```git remote rename <old-name> <new-name>```
- Pushing to Git remotes
- ```git push <remote-name> <branch-name>```
 
## Git Language
- C language
## Git Stages
- Working Area
- Untraked
- Staged
- Commited
- Modified
## Git Repository
- Git repository is a place where our files can be stored
- we need to create a repository from github
- we can create folder and intialize with git init

## Bare Repository
## Conflict
- Conflict arrives when any two or more devlopers are working on same file any one might have conflict
- to resolve need to disuss with each other and changes the file accordingly then back to push again to main

## Git Commands
#### Rename brnach
```
checkout to branch
git branch -m <new-branch-name>
```
```
without checkout to branch
git branch -m <branch-name><new-branch-name>
```
```
git push origin -u <new-branch-name>
git push origin -d <old-branch-name>
```
## Git Config
```
git config --global user.name
```
```
git config --global user.email
```
```
git config --global user.name <your_name>
```
```
git config --global user.email <your_email>
```

## Forking
- it is just like a  Git Clone
- It is widely used in Open Source
- we can clone any repository from hub called as Forking

## Senario Questions

