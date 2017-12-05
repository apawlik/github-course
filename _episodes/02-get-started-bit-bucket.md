---
layout: episode
title: "Getting started with BitBucket"
teaching: 5
exercises: 0
questions:
- "How to contribute to an existing repository on BitBucket?"
objectives:
- "Learning how to clone a repository on BitBucket."
- "Learning how to add collaborators to the project."
- "Understanding different repository setups and write access on BitBucket."
keypoints:
-   "Learning how to clone a repository and request/give access to collaborators."
permalink: /02-get-started-bit-bucket
---

You may find yourself wanting or needing to contribute to code base that already exists and has a number of contributors working on it. One of the places where the code can be hosted is a repository in [BitBucket](https://bitbucket.org/). BitBucket is a hosting service allowing that can be used for hosting source code along with a number of tools which support collaboration on the said code (such as a wiki, issue tracker and more). What is important is that the source code is hosted in either Git or Mercurial repositories. Shortly speaking, BitBucket provides the functionality of version control system together with some additional services which make it extremely useful in collaborative work.

For the purpose of our training we will use a [copy of New Zealand Government repository](https://bitbucket.org/apawlik/public-sector-websites) containing information about public sector websites. The [original of this repository is actually hosted on GitHub](https://github.com/GOVTNZ/public-sector-websites) (which is a service similar to BitBucket). But as in this module we want to learn how to use BitBucket, we will go with a copy.

### Create a BitBucket account

Go to [BitBucket](https://bitbucket.org/account/signup/) website and create an account. NOte down your username - you will need it. Then log in.
You should see a dashboard similar to this one:


### Set up for cloning

If you are using Windows, please start GitBash. If you are using Mac or Linux, please start the Terminal (you will be able to find it in Applications on Mac).

### Clone the repository

Go to our sample (but real) [repository](https://bitbucket.org/apawlik/public-sector-websites). On the left hand side you should see a plus sign. Click on it and you should see a submenu with a section `GET TO WORK`. Below you should see `Clone this repository` (see the image below).


When you click on `Clone this repository`, you will see a pop-up window.


Copy the address that is visible next to `HTTPS` (see below).

Now go to your terminal and paste the line you copied. In GitBash Ctrl+V will **not** work. You need to right click and then select `Paste`.

```
git clone https://apawlik@bitbucket.org/apawlik/public-sector-websites.git
```

You should see a similar output:

```
Cloning into 'public-sector-websites'...
remote: Counting objects: 224, done.
remote: Compressing objects: 100% (91/91), done.
remote: Total 224 (delta 130), reused 224 (delta 130)
Receiving objects: 100% (224/224), 126.06 KiB | 223.00 KiB/s, done.
Resolving deltas: 100% (130/130), done.
```

Now you should have the exact clone of the repository on your machine. Type:

```
cd public-sector-websites
```
