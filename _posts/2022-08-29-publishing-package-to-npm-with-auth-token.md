---
layout: post
title: Yoga instills mindfulness
description: Elevate your Eonsciousness
imageUrl: /assets/images/monopteros.jpg
---

## Step 1
Get a **publish** token from your account : https://docs.npmjs.com/creating-and-viewing-access-tokens

## Step 2
Add `.npmrc` file to your project root with the following contents by replacing `your-access-token` with the token you got in step 1.

```.npmrc
//registry.npmjs.org/:_authToken=your-access-token
```
Source : https://docs.npmjs.com/using-private-packages-in-a-ci-cd-workflow#create-and-check-in-a-project-specific-npmrc-file

## Step 3
Bump the version and publish the package
```sh
npm version patch # to bump the version.  You can use major, premajor, minor, preminor, patch or prepatch here depending on your changes.
npm publish --access public # to publish the package
```

Thats All Folks!!!
