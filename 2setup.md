---
layout: default
title: 2-Setup
---

# First Time Setup and Configuration

To start learning Git we will use it on the command line.
Although there are GUI clients to manage Git repositories, being familiar with the command line version will help you better understand the basic workflow.
If you need a command line refresher, check out this [mini-lesson](https://evanwill.github.io/_drafts/notes/commandline.html).
So fire up your favorite shell, terminal, or Git Bash to get started!

## Git Config

Some initial setup is necessary the first time you use Git on a computer.
You will use these commands only once, unless you want to change something.

Set your name and email:

```
git config --global user.name "Evan Will"
git config --global user.email "myemail@gmail.com"
```

Set your default text editor (Windows "notepad", Mac "edit -w", Linux "nano -w"):

```
git config --global core.editor “notepad”
```

> Your email and user name is recorded with every commit.
> This helps ensure integrity and authenticity of the history.
> Most people keep their email public, but if you are concerned about privacy, check GitHub's tips to [hide your email](https://help.github.com/articles/keeping-your-email-address-private/).

## Create repository locally

To try Git out, create a local repository:

```
mkdir test

cd test

git init
```

Your new directory `test` will have a hidden `.git` directory which will contain the full history. 
It is hidden for a reason--you don't need to know anything about it!
If you want to add this repository to GitHub, you have to `git remote add`.

## Create repository on GitHub

A more common workflow is to create or fork a repository on GitHub, then `clone` it to your local machine.
GitHub acts as Git in your browser, with added benefits.
Create a new remote repository:

- Login to [GitHub](https://github.com/) 
- Click the plus sign on the upper right and select "New repository" from the drop down
- Give it a nice name
- Check "Initialize this repository with a README"
- Click "Create repository"

With this test repository ready, we can move on to the basic Git workflow!
