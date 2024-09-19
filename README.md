# Fetch all và xóa nhánh local
```
git fetch --all
git checkout main
git branch | grep -v "main" | xargs git branch -D
```
