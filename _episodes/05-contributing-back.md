---
layout: episode
title: "Contributing back your changes"
teaching: 25
exercises: 2
questions:
- "How to contribute back your changes to an existing project?"
objectives:
- "Know how to use commands such as git commit and git push to contribute changes."
keypoints:
-   ""
permalink: /05-contributing-back/
---

After we made some changes to the project, we need to record them with the version control. Let's see what Git knows about our work:

```
   $ git status
```

We need to tell Git to track the new file and add it to the [staging area](http://swcarpentry.github.io/git-novice/04-changes/#staging-area) so that it can be committed. 

```
   $ git add
```

```
   $ git commit
```

```
   $ git push
```


Exercise 1:

Add a file named the following way: your initials and month of birth (so for example `anp02.txt` - we want everyone to create a file with a different name) to the repository. Commit these changes and push them to the remote repository.