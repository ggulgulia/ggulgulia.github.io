---
layout: post
title: How to execute command on changing any files in NodeJS environment?
description: As simple as it gets
imageUrl: assets/images/Anokhi-Group-1.jpeg
---

The simplest way to execute a command on file change is:

```sh
nodemon -e ts,env --exec "echo hello"
```

The `-e` flag is to configure the `extensions - for ex. ts, js, env, etc.` and `--exec` executes the command when file with 
the configured extension changes.

For more information visit this [npm nodemon package](https://www.npmjs.com/package/nodemon).
