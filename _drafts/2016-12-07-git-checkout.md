---
layout: post
title: "git checkout"
description: ""
category: Programming
tags: [ git, tips]
---
**When to use**: If you want to work with branches or restore locally deleted files. 
**When not to use**: If you want to work with a new or existing repository. See (git clone)[https://peterabarry.github.io/programming/2016/12/07/git-clone].
**How to use**: A few cases that come up.

1) `git checkout <branch>` - start working on that branch. 

2) `git checkout -b <branch>` - create the branch locally. ( Still need more steps to share this remotely).

3) `git checkout <tag>` - checkout a tagged commit which may not be the tip of any branch. HEAD is now detached.

5) `git checkout <commit> <file>` - revert the file to the commit referenced by <commit>

6) `git checkout <file>` - get back a file from the index. (e.g. restore a deleted file)

7) `git checkout -- 'glob pattern' - get pack all files matching pattern from index. (e.g. restore deleted files).

8> `git checkout -m <branch>` - switch to branch and do a 3 way merge between the local changes on the prev branch, the requested branch and the current HEAD of the origin of the new remote. 

{% include JB/setup %}


