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
```
git pull is a Git command used to update the local version of a repository from a remote.
git pull fetches (git fetch) the new commits and merges (git merge) these into your local branch.
```
## Git Pull Request
```
A pull request is an event in Git where a contributor asks a maintainer of a Git repository to review code they want to merge into a project.
The process for a pull request approval in Git will involve getting the project maintainer(s) to review your work; after which they will provide comments or, if your pull request is approved, will merge your changes directly into the main repository. 

```
## Git Fetch
```
git fetch is the command that tells your local git to retrieve the latest meta-data info from the original (yet doesn’t do any file transferring. It’s more like just checking to see if there are any changes available).

```
## Git Merge
```
1. Merge
2. Fast Farward Merge (likely Rebase)
3. 3-way Merge
The git merge command lets you take the independent lines of development created by git branch and integrate them into a single branch.
```
## Git Rebase
```
Rebasing is the process of moving or combining a sequence of commits to a new base commit. Rebasing is most useful and easily visualized in the context of a feature branching workflow.
```
## Git Revert
```
The git revert command is a forward-moving undo operation that offers a safe method of undoing changes.
git revert HEAD [main b9cd081]
```
## Git Reset
```
The git reset command is a complex and versatile tool for undoing changes. It has three primary forms of invocation. These forms correspond to command line arguments --soft, --mixed, --hard.
git reset filename
git reset --soft filename
git reset --hard filename
git reset --mixed filename
```
## Git Stash
## Git Stash Apply
## Git Stash drop
## Git diff
## Git status
## Git Cherrypick
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

