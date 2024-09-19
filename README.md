# Fetch all and delete local braches
```
git fetch --all
git checkout main
git branch | grep -v "main" | xargs git branch -D
```
or with powershell on window
```
git branch | ForEach-Object { $_.Trim() } | Where-Object { $_ -ne 'main' } | ForEach-Object { git branch -D $_ }
```

# View latest commits
```
git log -1 --oneline
```
