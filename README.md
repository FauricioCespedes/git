# git

## Alias

### Git Status
git config --global alias.s "status -s"

### Git Log
git config --global alias.l 'log --pretty=format:"%C(bold yellow)%h%C(reset) - %C(cyan)%cr%C(reset) - %s"'

### Git Fetch Prune
git config --global alias.fp 'fetch --prune'

### Git Add & Commit
git config --global alias.ac '!git add -A && git commit -m'

### Git Branch Cleaning Up
git config --global alias.bc '!git fetch -p && git branch -vv | awk "/: gone]/{print \$1}" | xargs -r git branch -d'
