---
title: How to create a worktree in Git?
description: This post will clarify on how to have 2 folders for the same Git project.
imageUrl: https://user-images.githubusercontent.com/12084821/192946383-e2d754ff-20a4-42d5-8ce2-880f85accaba.jpg
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
