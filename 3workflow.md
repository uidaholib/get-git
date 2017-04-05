---
layout: default
title: 3-Workflow
---

# Basic Git Workflow

`git clone... / pull`

Edit files

```
git add...
git commit...
git push...
```

## Track a file [ git add ]

git status
Git status is your friend. Type it often. Create a new file:
echo "some interesting notes" > notes.txt
git status
Start tracking the file with "git add", adding the file to the "staging area":
git add notes.txt
git status

## Commit [ git commit ]

We are ready to store a set of changes, let's commit!
A message is required and will be recorded along with name and date. It is your note to
posterity so you can remember what you did in the future.
git commit -m "add notes file"
git status
A commit is like a snap shot. We have stored away a new version of the documents in the
repository and we will be able to navigate this history.
Make many smaller focused commits, rather than big ones, since small changes will be
easier to undo, review, and merge.

## Repeat!

You will use "add", "commit", and "status" over and over!
Git add fills the staging area.
Git commit takes the snapshot of changes in the staging area.
git add notes.txt
git commit -m "more notes"
git status

## Send changes to GitHub [ git push ]

git status
Notice git status now says "your branch is ahead of origin/master".
We finished our changes to the repository locally, now we have to add them to the version
hosted on GitHub.
git push origin master
Origin/master is the standard way to name the main branch of the central repository.
Push sends only the commits, so it is efficient network use.

## Review basic workflow
git status
git pull origin master
git add file.txt
git commit -m "message"
git push origin master