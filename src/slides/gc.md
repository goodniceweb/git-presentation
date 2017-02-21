class: center, middle

# Git has his own garbage collector

<img src="img/gc.jpg" class="content-image">

???

Git stores all comressed file each time you do commit and then show diff to you between that files.

The optional configuration variable gc.reflogExpire can be set to indicate how long historical entries within each branch’s reflog should remain available in this repository. The setting is expressed as a length of time, for example 90 days or 3 months. It defaults to 90 days.

The optional configuration variable gc.reflogExpireUnreachable can be set to indicate how long historical reflog entries which are not part of the current branch should remain available in this repository. These types of entries are generally created as a result of using git commit --amend or git rebase and are the commits prior to the amend or rebase occurring. Since these changes are not part of the current project most users will want to expire them sooner. This option defaults to 30 days.

The optional configuration variable gc.rerereResolved indicates how long records of conflicted merge you resolved earlier are kept. This defaults to 60 days.

The optional configuration variable gc.rerereUnresolved indicates how long records of conflicted merge you have not resolved are kept. This defaults to 15 days.

---

