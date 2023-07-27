# Remove Already Committed From Gitignore

From [stack overflow](https://stackoverflow.com/questions/9750606/git-still-shows-files-as-modified-after-adding-to-gitignore)

If a file is already in the index with the `.gitignore` is updated, they will continue to be tracked. To remove them from the index, you can enter

```bash
git rm -r --cached {file_name}
```