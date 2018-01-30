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
**Exercise**:

Edit the file you created in the previous exercise - add your first name to it. Save it, commit your changes and push them into the repository.


### Resolving conflicts

What happens if two or more people edit the same part of the repository (the same file, in the same place)?

**Exercise**:
Edit the `README.md` file - at the very top of it write: *This is line one added by YOUR NAME*. Commit and push back your changes. 

If you were the first one pushing your changes, it will all work OK. But if not, then you will see a message similar to this one:

```
CONFLICT (content): Merge conflict in README.md
Automatic merge failed; fix conflicts and then commit the result.
```

Open the README.md file in the editor and see what you will find.

Once we finished editing the README.md file, we need to complete the *conflict resolution*.

```
  $ git add README.md
```

```
  $ git commit -am "Resolving the conflict"
```

Now try pushing back. What happens? How to get out of that situation?
