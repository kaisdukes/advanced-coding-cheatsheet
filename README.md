# Terminal Cheatsheet

🔥🔥 Essential terminal commands for Git and TypeScript. 🔥🔥

[Dr. Kais Dukes](https://github.com/kaisdukes)

## Git

### Clean display of git log

```
git log --pretty=format:"%C(yellow)%h %C(green)%ad %C(reset)%s" --date=format:"%Y-%m-%d %H:%M:%S"
```

### Check the git status of multiple repositories

```
find . -name .git -type d -execdir sh -c "pwd ;git status" \;
```

## TypeScript

### Type check without generating output

```
npx tsc --noEmit
```