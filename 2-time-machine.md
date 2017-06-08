# 时光机穿梭

## 1.查看

- 查看当前仓库状况，做了哪些修改

```
  git status
```

- 对比某个文件与上个commit的区别
```
  git diff filename
```

- 显示提交记录,后者在一行显示提交id和信息
```
  git log
  git log --pretty=oneline
```
## 2.版本回退
利用这个命令可以回退，但是相当危险，因为会丢弃commit和当前没有stage的东西。

HEAD表示当前版本，HEAD^表示上一个版本,以此类推HEAD~100,commitid也可以是这些。
```
git reset --hard commitid
```