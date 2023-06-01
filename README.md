# Terminal Cheatsheet

## Git

### Clean display of git log

```shell
git log --pretty=format:"%C(yellow)%h %C(green)%ad %C(reset)%s" --date=format:"%Y-%m-%d %H:%M:%S"
```

### Check the git status of multiple repositories

```shell
find . -name .git -type d -execdir sh -c "pwd ;git status" \;
```

## TypeScript

### Type check without generating output

```shell
npx tsc --noEmit
```