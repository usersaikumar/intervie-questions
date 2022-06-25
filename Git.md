# GIT
- Source Code Management
- Version Control System
- De-Centralized

## Branching Strategy
- Trunk Based
- Feature Branch
- Forking
- Release Branch
- Git Flow
- Env Branch
- GiHub Flow

### GitHub Flow
#### Creating a Branch
- Branches help you work on features, Fix bugs
- Do not effect master branch
- Anything in the master branch is deployable
#### Add Commits
- Keeps track of changes in your feature branch
- More transparent history of work
- A separate unit of change
#### Open a Pull Request
- Discussion about your commits
- Open it during any point of your development process
- You can ask feedback from any of your team members
- Pull request frame a problem by describing it
- Reviewer is aware of your problem statement
- A basic run through from setup to expected outcome is recommended
#### Discuss and Review your Code
- People reviewing your code might have feedback
- A review focusses on the code health and on production readiness
- Code health & Production Readiness
#### Test Your Changes
- Test in a production like Environment
- Update your tool
#### Merge your Feature
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
## Git diff
## Git status
## Git Remote
## Git Language
## Git Stages
## Git Repository
## Bare Repository
## Conflict

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
## Forking
## Senario Questions

