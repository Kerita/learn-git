# learn-git

## 目录
1.[删除和重命名远程分支](#删除和重命名远程分支)

2.[新建分支](#新建分支)

## 1.删除和重命名远程分支
> 重命名远程分支，其实是先把远程分支删除，然后重命名本地分支，并推到远程仓库。

>以imporve重命名为improve为例,查看所以分支,删除远程分支,重命名本地分支,推送本地分支。

```
  git branch -av
  git push --delete origin improve
  git branch -m imporve improve
  git push origin improve
```

## 2.新建分支
> master分支维持稳定，自己切一个分支进行开发，上线的时候，将自己的代码合并到master上，并在master上打tag
```
  git branch dev
  git checkout dev
  git push origin dev
```



