class: center, middle

# Aliases

```
[alias]
  co = checkout
  br = branch
  ci = commit
  st = status
  fixtypo = commit --amend --no-edit
  resetmerge = reset --merge ORIG_HEAD
  cleanup = "!git branch --merged | grep  -v '\\*\\|master\\|develop' | xargs -n 1 git branch -d"
  patch="!git format-patch -1 HEAD"
```


---
