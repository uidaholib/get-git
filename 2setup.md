---
layout: default
title: 2-Setup
---

# First Time Setup and Configuration

Shell
terminal, command
line, Bash, etc
An application that lets you communicate with your
operating system.

Command-line interface (CLI)
read-evaluate-print loop (REPL)
On Windows use Git Bash for Unix-like commands
so you can follow Mac or Linux tutorials.

https://evanwill.github.io/_drafts/notes/commandline.html

## Git Config
one time initial
setup
Set your name and email:
git config --global user.name "Evan Will"
git config --global user.email "myemail@gmail.com"
Set your text editor (Windows "notepad", Mac "edit -w", Linux "nano -w"):
git config --global core.editor “notepad”

Worried about privacy, see https://help.github.com/articles/keeping-your-email-address-private/

## Create repository locally

mkdir test
cd test
git init
Your new folder "test" will have a hidden folder ".git" which contains the full history. It is
hidden for a reason--you don't need to know anything about it!
If you want to add this repository to GitHub, you have to "git remote add".
For most basic workflows it is easier to start a repository on GitHub, then "clone" it to your
local machine.

## Create repository on GitHub

GitHub
git repository hosting
service
Use Git in a web browser!
Create a Repository:
● https://github.com/
● Log in
● Click + to create new repository
● Name it
● Click initialize with README
● Click "Create repository"
Create a commit:
● Click on a file
● Edit in browser
● Scroll down to "Commit changes"
● Fill in the information describing the change
● Click "Commit changes"

## Clone repository from GitHub

Go to your GitHub repository,
Click “clone or download” button,
Copy the clone url.
git clone https://github.com/uidaholib/gitworkshop.git
Clone will download a full copy of the repository to your local machine and
record its origin on GitHub. This ensures there is a connection so you can
Push your changes to GitHub or Pull updates.
Your clone has the full history stored in the ".git" hidden folder.