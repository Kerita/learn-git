# learn-git

## 目录
1.[删除和重命名远程分支](#删除并重命名远程分支)




## 1.删除并重命名远程分支
> 重命名远程分支，其实是先把远程分支删除，然后重命名本地分支，并推到远程仓库。

```
  // 以将imporve重命名为improve为例
  // 查看所以分支
  git branch -av
  // 删除远程分支
  git push --delete origin improve
  // 重命名本地分支
  git branch -m imporve improve
  // 推送本地分支
  git push origin improve
```



