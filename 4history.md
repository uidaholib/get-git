---
layout: default
title: 4-History
---

## History [ git log ]

Check how far we have come! Take a look at the repository's history of commits.
git log
git log --oneline

## Check changes [ git diff ]

Now modify one of the file in your repository using a text editor or the CLI.
echo "more important notes!" >> notes.txt
git status
git diff
Diff allows us to see what changes were made to the currently unstaged files. Its best to
check this before you commit to ensure you know what you are changing.


## Undo [ git checkout ]

Wait that last commit was no good! Let's get the earlier version back.
You can track individual commits using their id given by git log. Or we can refer to them
sequentially. The most recent commit is called "HEAD". One back is called "HEAD~1"
(head minus one). If you git checkout a specific file, it will reset it to that commit.
git checkout HEAD~1 notes.txt
git diff HEAD notes.txt
git checkout HEAD notes.txt
These two checkouts undid each other!
[ if you get 'detached HEAD' warning, type "git checkout master" ]
