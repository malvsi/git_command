## git基本操作
> 查看文件状态
> 
``` bash
git status
```

> 添加文件
> 
```bash
git add [filename]
```

> 添加描述
> 
```bash
git commit -m '提交描述'
```

> 第一次提交文件到远程仓库
> 
```bash
git push -u origin master
```

> 提交文件到远程仓库
> 
```bash
git push origin master
```

## 基本信息设置
> 设置用户名
> 
```bash
git config --global user.name 'your user name'
```

> 设置用户名邮箱
> 
```bash
git config --global user.name 'useremial@qq.com'
```

> 查看git配置信息
> 
```bash
git config --list
```

## 分支操作
> 查看分支，*代表当前分支
> 
```bash
git branch -a
```

> 新建分支
> 
```bash
git branch [branch name]
```

> 切换分支
> 
```bash
git checkout [branch name]
```

> 删除本地分支
> 
```bash
git branch -d [branchname]
```

> 删除远程分支
> 
```bash
git push origin --delete <branchname>
```

> 合并分支
> 
```bash
git merge [branch name]
```

## git remote的操作
> 查看远程关联仓库
> 
```bash
git remote -v
```

> 删除远程关联仓库
> 
```bash
> <name> == origin
git remote remove <name> 
```

> 添加远程关联仓库
> 
```bash
git remote add origin <url>
```

> 修改远程关联仓库（地址）
> 
```bash
git remote set_url <name> <newurl>
```

## git clone的操作
> 克隆远程仓库
> 
```bash
git clone <url>
```

> 克隆远程仓库并重命名文件夹
> 
```bash
git clone <url> <filename>
```