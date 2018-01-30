---
layout: episode
title: "Reviewing changes and history in your repository"
teaching: 20
exercises: 0
questions:
- "How to view the changes made to files in the repository?"
- "How to discard changes you made?"
objectives:
- "Know how to browse history in the repository."
- "Discarding unwanted changes."
keypoints:
-   "."
permalink: /04-browsing-history/
---

Let's have a look what has been going on in this particular repository:

```
   $ git log
```

You should see output similar to this one:

```
commit 51ef8b80ec9577de5650c1def7e69f313efb3f8f (HEAD -> master, origin/master, origin/HEAD)
Merge: 123f84d 09e0349
Author: Cam Findlay <info@camfindlay.com>
Date:   Mon Sep 11 13:02:21 2017 +1200

  Merge pull request #35 from racheljdavis/patch-15

  MFE updates

commit 09e0349bb5ae37e76d3079fefdf659b6a39fb503
Author: Rachel Davis <racheljdavis@users.noreply.github.com>
Date:   Mon Sep 11 10:59:34 2017 +1200

  MFE updates

  re: Kyla Huff's amendments

commit 123f84d45114ba9dfbd0f608b5606cf092d93236
Author: Cam Findlay <info@camfindlay.com>
Date:   Mon Sep 11 10:55:34 2017 +1200

  Add snapshot for 30 June 2017

commit 0702f4ee26aaa83d91687db920091c205aae631f (tag: 2017-06-30)
Merge: 9702b98 443fb86
Author: Cam Findlay <info@camfindlay.com>
Date:   Mon Sep 11 10:40:33 2017 +1200

  Merge pull request #33 from racheljdavis/patch-13

  Update Crown Fibre Holdings

commit 9702b9814c29bf4010d2d9963349d948bff708ec
Merge: 5648476 eace540
Author: Cam Findlay <info@camfindlay.com>
Date:   Mon Sep 11 10:37:52 2017 +1200

    Merge pull request #31 from racheljdavis/patch-11

    Update Porirua City Council
```

Let's see what's actually been done in the commit which had a message "Update Porirua City Council"

```
  $ git diff 9702b
```

The output is very long (as there were several things added) so below we just pick up a part of the output so that we can have a closer look:

```
diff --git a/data.json b/data.json
index 762d064..d9e5cc0 100644
--- a/data.json
+++ b/data.json
@@ -10,7 +10,7 @@
                        "landingPage": "https://github.com/GOVTNZ/public-sector-websites",
                        "identifier": "https://github.com/GOVTNZ/public-sector-websites",
                        "issued": "2011-08-26",
-                       "modified": "2017-04-08",
+                       "modified": "2017-09-11",

```

Cloning not only copies the files but brings in the full functionality of the repository.
