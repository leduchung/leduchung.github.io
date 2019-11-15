---
title: "A brief of Git usage"
categories:
 - devops
tags:
 - git
last_modified_at: 2019-11-08
---

Not so many documentations about [Git](https://git-scm.com/) mention about the remote-tracking references. Here we can revise how Git work with remote.

# Git is distributed

We all know that Git works as a distributed model. That means, a repository, regardless it is on your machine or somewhere else, will contain all possible information. Data can be transfer between Git nodes. One Git can play the role of the server and others as clients, but there are no differences internally.

# The git local and git remote

The below diagram has several common versions on the Internet. I want to summary these steps and emphasize the remote-tracking reference which is usually overlooked.

<div class="mxgraph" style="max-width:100%;border:1px solid transparent;" data-mxgraph="{&quot;highlight&quot;:&quot;#000000&quot;,&quot;lightbox&quot;:false,&quot;nav&quot;:true,&quot;toolbar&quot;:&quot;layers&quot;,&quot;edit&quot;:&quot;_blank&quot;,&quot;xml&quot;:&quot;&lt;mxfile host=\&quot;www.draw.io\&quot; modified=\&quot;2019-11-15T10:30:07.020Z\&quot; agent=\&quot;Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/78.0.3904.97 Safari/537.36\&quot; etag=\&quot;zzcg4RdgRVWUjc2G4cxK\&quot; version=\&quot;12.2.6\&quot; type=\&quot;device\&quot; pages=\&quot;1\&quot;&gt;&lt;diagram name=\&quot;Page-1\&quot; id=\&quot;13e1069c-82ec-6db2-03f1-153e76fe0fe0\&quot;&gt;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&lt;/diagram&gt;&lt;/mxfile&gt;&quot;}"></div>
<script type="text/javascript" src="https://www.draw.io/js/viewer.min.js"></script>


## A straight route to the remote server

When you have work done, then the most common git commands in action would be the triad:

```bash 
git add
git commit
git push
```

You do it daily when you understand well your task and when you work alone in a branch. In simple words, your code goes from your keyboard to the remote server.

## The bridge between remote and local

There are two middle areas:
 - The `local refs` is a buffer for your local before pushing
 - The `remote-tracking refs` is a buffer for your remote before pulling

Then, you will see the [`git commit`](https://git-scm.com/docs/git-commit) and [`git fetch`](https://git-scm.com/docs/git-fetch) are symmetry and serving as two sizes of the bridge between local and remote repository. Right on that bridge, annoying conflicts might happen. If you do [`git pull`](https://git-scm.com/docs/git-pull), first `git fetch` will be executed, then the merging process and conflict solving will follow. `Git pull` will let you fix your conflict a the code level, but `git fetch` let you investigate the conflict (on the bridge) before any action.

```
"git pull" = "git fetch" AND [("git checkout" if no conflict) OR (git merge if there is any conflict)]
```

 - You do `git fetch` to update the remote-tracking references, which means you won't see any change in your repository yet but only download the remote data.


<img style="float: right;" width="200" src="https://pics.me.me/in-case-of-fire-1-git-commit-2-git-push-32731112.png">

## The backup area

The `stash` area is not a common but still an useful feature. When you think your code is crap (yes it is) and you must delete it but hesitate to do so, then do [`git stash`](https://git-scm.com/docs/git-stash) to save you changes and reversed your unstaged work.

## The best documentation of Git

The Internet created a large number of documents about it. I prefer using the [official site](https://git-scm.com/docs), which is short and complete. Sometimes, Stackoverflow can work well to find a quick solution. Other resources, I think, only re-cook the material from the official site to make it more engageable to the reader. So this blog is, too.