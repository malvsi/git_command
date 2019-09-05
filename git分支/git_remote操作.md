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