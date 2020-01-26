# Basic Git workflows
This document is to describe various git workflows.

## Basic questions

### How do I get my local changes into Github?
1. Check the status of your local repository
    - In your git repository run: `git status`
    - What you should be looking for:
        1. Are you on the branch you expect to be?
        1. Are the changes that you want included showing up?
        1. Are there any changes that you *DON'T* want showing up?
1. Stage the files that you want to include in your commit by running: `git add {fileName}`. Only staged files will be committed, so stage all the files that you want updated, and don't stage anything that you don't want updated.
    - To include all changed files, run: `git add -A`
        - To check which files will be added: run `git status` first
1. Verify that the files that you want to commit are staged.
    - Run: `git status`
1. Commit your changes. Be sure to a descriptive message so your future self will know what this commit is for. Your future self will thank you later.
    - Run: `git commit -m "{your commit message}"`
1. Push your commits.
    - Run: `git push`
    - If you get an error that there is no upstream branch, do not fret. Set your upstream branch: `git push --set-upstream origin {name-of-branch}`

Note:
- You can combine steps 1 and 2 with this command: `git commit -am "{your commit message}"`
    - `git commit -am` is pretty much `git add -A` with `git commit -m`

### How do I create a new branch?
1. Make a local branch by running: `git branch {branchName}`

Creating a local branch does not mean that you are automatically working in that branch. To start working in that branch you will need to _checkout_ the branch by running: `git checkout {branchName}`.

But there's a better way to do this since it's such a common workflow!

1. Make a local branch **AND** checkout that branch by running: `git checkout -b {branchName}`