## Git -> starting
```
git init -b main
```

## Git Submodules

### Adding
```
git submodule add <link>
```

#### Updating
```
git submodule update --remote --merge
```
or
```
git submodule foreach git pull
```
and then `git add` the folder

### Removing
\#Remove the submodule entry from .git/config
git submodule deinit -f path/to/submodule

\#Remove the submodule directory from the superproject's .git/modules directory
rm -rf .git/modules/path/to/submodule

\# Remove the entry in .gitmodules and remove the submodule directory located at path/to/submodule
git rm -f path/to/submodule

## Ammending
```
git add <file>
git commit --amend --no-edit
```
To change commit-message remove `--no-edit`
