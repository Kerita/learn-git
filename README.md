# learn-git

## 目录
1.[删除和重命名远程分支](#1.删除和重命名远程分支)

2.[新建分支](#2.新建分支)

3.[新建tag与删除tag](#3.新建tag与删除tag)

4.[删除某个远程文件但不删除本地文件](#删除某个远程文件但不删除本地文件)


## 1.删除和重命名远程分支
重命名远程分支，其实是先把远程分支删除，然后重命名本地分支，并推到远程仓库。

以imporve重命名为improve为例,查看所以分支,删除远程分支,重命名本地分支,推送本地分支。

```
  git branch -av
  git push --delete origin improve
  git branch -m imporve improve
  git push origin improve
```

## 2.新建分支
master分支维持稳定，自己切一个分支进行开发，上线的时候，将自己的代码合并到master上，并在master上打tag
```
  git branch dev
  git checkout dev
  git push origin dev
```

## 3.新建tag与删除tag

```
git tag -a tagname -m "taginfo"
git push origin tagname
git tag -d tagname
git push origin --delete tag tagname
```

## 4.删除某个远程文件但不删除本地文件

提交的时候忘记把文件路径添加到.gitignore中，不小心把文件提交上去，怎么办呢？

把这个文件加到`.gitignore`里面忽略掉，然后提交使.gitignore生效

```
git rm -r --cached .
git add .
git commit -m "ignore take effect"
git push origin master
```

## 5.测试git-extra
```
  git changelog
```

## 


