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

## git基本操作
> 查看文件状态
> 
``` bash
git status
```

> 添加文件
> 
```bash
git add <filename>
```

> 直接提交文件 [-a]可以跳过 add 添加过程直接提交
> 
```
git commit -a -m '描述信息'
```

> 查看文件哪里被更新
> 
```
git diff
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

# 文件操作
## 移除文件
> 移除文件
> 
```bash
git rm <filename>
```

> 强制移除文件
> 
```bash
git rm -f <filename>
```

> 移除某个目录下的文件 正则表达式
> 
```bash
git rm src/\*.html   // '移除src文件下所有.html文件'
git rm \*~			// '移除已～结尾的文件'
```

> 移除仓库文件，但在本地保留
> 
```bash
git rm --cached <filename>
```

## 移动文件
> 移动文件
> 	
```
git mv <file_from> <file_to>
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

## 查看提交历史
> 查看提交历史
> 
```
git log
```

> 查看提交的内容差异 -p，查看最近两次提交的内容差异和历史
> 
```
git log -p -2
```
