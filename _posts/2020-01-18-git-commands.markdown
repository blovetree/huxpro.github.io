---
layout:     post
title:      "Git Commands"
date:       2019-11-06
author:     "Dylan"
header-img: "img/post-git-commands.jpg"
catalog: true
tags:
    - Git
    - Commands
---


#### untracked files

```
git clean -f    #删除 untracked files
git clean -fd   #连 untracked 的目录也一起删掉
git clean -xfd  #连 gitignore 的untrack 文件/目录也一起删掉。
                #慎用，一般这个是用来删掉编译出来的 .o之类的文件用的
```

在用上述 git clean 前，建议加上 -n 参数来先看看会删掉哪些文件，防止重要文件被误删

```
git clean -nxfd
git clean -nf
git clean -nfd
```


#### 撤销add

`git reset`


#### 撤销没add修改

`git checkout .`


#### Please move or remove them before you switch branches

`git clean -dfx`