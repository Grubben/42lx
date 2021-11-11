## Git Submodules

### Adding
```
git submodule add <link>
```

#### Updating
```
git submodule update --remote
```
or
```
git submodule foreach git pull
```
and then `git add` the folder

## Ammending
```
git add <file>
git commit --amend
```
