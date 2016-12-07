---
layout: post
title: "git checkout"
description: ""
category: Programming
tags: [ git, tips]
---
##### When to use:
If you want to work with branches. 
##### When not to use:
If you want to work with a new or existing remote repository.
See git clone.

##### How to use:
**git checkout** needs a [URL](https://en.wikipedia.org/wiki/Uniform_Resource_Locator#Syntax) to clone. git supports [these URL schemes](https://git-scm.com/book/en/v2/Git-on-the-Server-The-Protocols).

Verbartim from `git help clone`:

>       Git supports ssh, git, http, and https protocols (in addition, ftp, and
>       ftps can be used for fetching and rsync can be used for fetching and
>       pushing, but these are inefficient and deprecated; do not use them).
>
>       The native transport (i.e. git:// URL) does no authentication and
>       should be used with caution on unsecured networks.
>
>       The following syntaxes may be used with them:
>
>       ·   ssh://[user@]host.xz[:port]/path/to/repo.git/
>
>       ·   git://host.xz[:port]/path/to/repo.git/
>
>       ·   http[s]://host.xz[:port]/path/to/repo.git/
>
>       ·   ftp[s]://host.xz[:port]/path/to/repo.git/
>
>       ·   rsync://host.xz/path/to/repo.git/
>
>       An alternative scp-like syntax may also be used with the ssh protocol:
>
>       ·   [user@]host.xz:path/to/repo.git/

##### When **git clone** fails

 1)  I got ```Permission denied (publickey).```
 A:  Probably you did not setup your SSH keys correctly, e.g. for [GitHub](https://help.github.com/articles/generating-an-ssh-key/) 

{% include JB/setup %}


