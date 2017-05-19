---
layout: default
title: Git Bash Bug
---

# Git Bash Bug
 
With some newly installed versions of Git Bash on Windows 10, your first attempt at `clone` results in an error message about not being able to do "https". 

In my experience, if you manually type in the clone URL (rather than pasting it in to the terminal) git clone will work.
Oddly, you only have to do it **one time**.
After the first successful clone, pasting the URL will work fine.

I know it sounds bizarre! But it works and I haven't been able to debug the issue any further.

(Back to [Workflow](../3workflow.html))