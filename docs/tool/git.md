# GIT

## 参考

[gitee命令](https://gitee.com/all-about-git)

[常用 Git 命令清单](https://www.ruanyifeng.com/blog/2015/12/git-cheat-sheet.html)


## 配置

1. 查看所有的配置以及它们所在的文件
```
git config --list --show-origin
```

1. 用户信息
```
git config --global user.name "John Doe"
git config --global user.email johndoe@example.com
```

1. 检查配置信息
```
git config --list
```

## 使用

### 增加/删除文件


1. 添加指定文件到暂存区
```
git add [file1] [file2] ...
```

1. 添加当前目录的所有文件到暂存区
```
git add .
```

1. 删除工作区文件，并且将这次删除放入暂存区
```
git rm [file1] [file2] ...
```

### 代码提交

1. 提交暂存区到仓库区
```
git commit -m [message]
```

1. 重写上次提交，可重写message
```
git commit --amend -m [message]
```

### 分支

1. 列出所有本地分支和远程分支
```
git branch -a
```

1. 删除分支
```
git branch -d [branch-name]
```

1. 删除远程分支
```
git push origin --delete [branch-name]
git branch -dr [remote/branch]
```

### 远程同步

1. 下载远程仓库的所有变动
```
git fetch [remote]
```

1. 显示所有远程仓库
```
git remote -v
```

1. 增加一个新的远程仓库，并命名
```
git remote add [shortname] [url]
```

1. 上传本地指定分支到远程仓库
```
git push [remote] [branch]
```

1. 强行推送当前分支到远程仓库，即使有冲突
```
git push [remote] --force
```

1. 推送所有分支到远程仓库
```
git push [remote] --all
```