# Whitespace

## Git

### Merge

```shell
$(master) git merge -Xignore-all-space origin/master
```

### Rebase

```shell
$(a-cool-feature) git rebase -Xignore-all-space master
```

## Github

Add `?w=1` to the URL to see the diff with whitespace ignored.

## Editors

### Vim

http://vim.wikia.com/wiki/Remove_unwanted_spaces

### Sublime Text 2

{
  "trim_trailing_white_space_on_save": true
}

### Xcode

http://stackoverflow.com/a/11830067/656428