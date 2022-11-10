---
title: Energize your inner core
description: Be aware of yourself and your sorroundings
imageUrl: assets/images/yoga-lotus.jpg
---

Photo by <a href="https://unsplash.com/@jannerboy62?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Nick Fewings</a> on <a href="https://unsplash.com/s/photos/2-roads?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Unsplash</a>
  
Sometimes, we may want to run the same Git project in 2 separate folders.  This is when `git worktree` comes to the rescue:

```sh
git worktree add ../project-worktree v2 # v2 is branch name and ../project-worktree is the new git-project-folder
```

To remove the worktree, simply:
```sh
git worktree remove ../project-worktree
```
