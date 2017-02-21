class: center, middle

# Aliases

```
[alias]
  a = add
  c = commit
  d = diff
  s = status
  co = checkout
  cob = checkout -b
  br = branch
  fixtypo = commit --amend --no-edit
  resetmerge = reset --merge ORIG_HEAD
  cleanup = "!git branch --merged | grep  -v '\\*\\|master\\|develop' | xargs -n 1 git branch -d"
  patch="!git format-patch -1 HEAD"
  lbr = "!git for-each-ref --sort='-authordate' --format='%(refname)%09%(objectname:short)%09%(authordate)' \
    refs/heads | sed -e 's-refs/heads/--' | column -t"
```


---
