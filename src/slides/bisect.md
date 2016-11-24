class: center, middle

# Bisect

This command uses a binary search algorithm to find which commit in your project’s history introduced a bug.

```
git bisect start [--term-{old,good}=<term> --term-{new,bad}=<term>]
    [--no-checkout] [<bad> [<good>...]] [--] [<paths>...]
git bisect (bad|new) [<rev>]
git bisect (good|old) [<rev>...]
git bisect terms [--term-good | --term-bad]
git bisect skip [(<rev>|<range>)...]
git bisect reset [<commit>]
git bisect visualize
git bisect replay <logfile>
git bisect log
git bisect run <cmd>...
git bisect help
```

---
