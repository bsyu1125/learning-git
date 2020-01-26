# Git Terminology
This page is to provide definitions for different Git terminology.
This page is not meant to be used for defining different Git commands (`git push`, `git pull`, etc) although they may overlap since some definitions for the terms are based on the command.
## Terms

### Branch

A parallel version of the repository. It is still part of the repository, and typically is used so that changes can be made and saved in a branch without affecting the `master` branch (or the "live" branch if it's not `master`). Once your body of work is done, you can merge the branch back into the `master` branch to publish changes

### Checkout

TODO

### Commit
As a noun: A single point in the Git history; the entire history of a project is represented as a set of interrelated commits. Also could be considered as a 'revision' or 'version'. Commits are 

As a verb: The action of storing a new snapshot of the project’s state in the Git history, by creating a new commit representing the current state of the index and advancing HEAD to point at the new commit.

### Diff
Diff stands for difference. Usually represents the differences between two commits or saved changes. The diff will visually describe what was added or removed from a file between the two commits.

### master
`master` is most commonly the name of a _branch_. This is *typically* the primary and "live" branch of the repository. 

In some git workflows, `master` is not the primary branch, so make sure you double check with the repository owners!

### Merge

TODO

### Repsitory
A repository contains all the project files and stores each file's commits in the project.

A repository is the result of the amalgamation of all the commits of a project.

Also called repo for shorthand.

#### Local Repository
The version of the repository on your local machine. You can pretty much do anything you want to your local repository and those changes will not affect any other version of the repository until you push those changes elsewhere.

#### Remote Repository
A version of the repository that is hosted remotely - typically hosted by Github. `origin` is the shorthand for a remote repository.

For example: run `git branch -a` to see all branches of a repo. Verify that every branch is active and is hosted on Github are preppended by `origin`.

### Push
Sending all committed changes to a remote repository. 

### Pull
Fetching and merging changes into your repository. If someone has edited the file remotely and you want those changes, you will want to pull in those changes.

### Fetch
Gets the latest changes from the remote repository without merging them into your local repository. Good way to view changes that were made to the remote repository.

## Useful External Links and References
- [Official Git Reference Docs](https://Git-scm.com/docs)
- [Github Git Cheatsheet](https://Github.Github.com/training-kit/downloads/Github-Git-cheat-sheet.pdf)