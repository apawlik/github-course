---
layout: episode
title: "Creating and using branches"
teaching: 20
exercises: 0
questions:
- "How can you create branch in Git?"
- "What are branches useful for?"
objectives:
- "Know how to create a branch in Git."
- "Understand why branches are useful."
keypoints:
-   "Using branches to contribute to research projects"
permalink: /06-branching/
---

Branching are useful for:

* making it easy to merge in changes contributed by multiple collaborators. 
* easily reviewing proposed changes (*one change = one branch*).
* keeping the master or release branch clean.
* making it easy to fix bugs and test before pushing into production code.
* making it easy for developing experimental new features.

Let's first create branch locally. Name the branch like the file in the previous exercises - your initials and month of birth, eg "anp02"

```
 $ git branch anp02
```

Let's move to that branch

```
 $ git checkout anp02
```

We can now do some development in this branch. Open the README.md file and add some text - wherever you want. Commit the changes.

Now we will push them back but creating a branch remotely:

```
  $ git push origin anp02:anp02
```
