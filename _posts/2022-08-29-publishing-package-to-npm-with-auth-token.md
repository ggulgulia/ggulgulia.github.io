---
layout: post
title: How to publish a NPM package with auth tokens?
description: As simple as it gets
imageUrl: https://user-images.githubusercontent.com/12084821/187110626-f09b8c2c-c0fe-4bf7-8efb-c55437b02f2d.jpg
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
