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
Let's start working with Git locally. First, we should see what Git is about now:

```
   $ git status
```

**Exercise**:

Add a file named the following way: your initials and month of birth (so for example `anp02.txt` - we want everyone to create a file with a different name) to the repository. 
After we made some changes to the project, we need to record them with the version control. Let's see what Git knows about our work:

```
   $ git status
```

We need to tell Git to track the new file and add it to the [staging area](http://swcarpentry.github.io/git-novice/04-changes/#staging-area) so that it can be committed. 

```
   $ git add anp02.txt
```

Now we can commit the file:

```
   $ git commit
```

And finally contribute back to the main repository:

```
   $ git push origin master
```

Depending how fast you were - you may need to first pull the changes (so update your local clone) and then push your changes:

```
   $ git pull origin master
```

