# source insight使用笔记


## windows端使用

1. 开启大小写敏感功能

选择一个目录，开启大小写敏感

```
fsutil file setCaseSensitiveInfo "D:\projects" enable
```

2. git配置，适配windows端

```
git config --global core.protectNTFS false
git config --global core.autocrlf true
git config --global core.filemode false
git config --global core.longpaths true
git config --global core.quotepath false
git config --global core.ignorecase false
```

注意：如果是从linux端拷贝的完整git仓库，在win解压后会出现始终无法区分大小写的情况，这时候只需要重新checkout

```
git clone FILETOGITDIR LOCALDIR
```

新建一个目录，从旧仓库中检出，将FILETOGITDIR作为服务端，FILETOGITDIR是目录路径



