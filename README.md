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







