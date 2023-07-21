# Advanced Coding Cheatsheet

🔥🔥 Step up your coding game with Git, TypeScript and AWS commands the internet has kept under wraps 🔥🔥

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

### Sleep for two seconds

```
await new Promise<void>(resolve => setTimeout(() => resolve(), 2000));
```

### One line text-to-speech generation

```
aws polly synthesize-speech --output-format mp3 --voice-id Emma --text "$(cat message.txt)" --engine neural --region us-east-1 message.mp3
```