class: center, middle

# Git Hooks

```
# Installation
#   ln -s /path/to/pre-commit.sh /path/to/project/.git/hooks/pre-commit
FILES_PATTERN='\.(rb|haml|coffee)(\..+)?$'
FORBIDDEN='binding.pry\|byebug'
 
git diff --cached --name-only | \
    grep -E $FILES_PATTERN | \
    GREP_COLOR='4;5;37;41' xargs grep --color --with-filename -n $FORBIDDEN && \
    echo "Looks like you are trying to commit something you shouldn't. \
      Please fix your diff, \
      or run 'git commit --no-verify' to skip this check, if you must." && \
    exit 1
 
exit 0
```

---
