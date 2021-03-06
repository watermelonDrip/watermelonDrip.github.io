---
title: 多终端同步功能实现 - Max
---

# 实现在多个终端上对博客进行更新和维护

*by max*

*2021/03/06*

为了方便多个管理员对博客网站的更新和维护，经过查询教程，实现了可以在两台电脑上各自分别利用hexo+git+github进行更新。
<!-- more -->

**本教程经过翻译并转自：**

`https://lanvoyager.github.io/posts/1bde756e/`

**侵删**

第一步：
此步骤请在原主机(已配置hexo环境并用于博客写作的电脑)上操作。

1. 进入blog所在主目录文件夹；(MacOS系统利用终端(terminal)cd进blog所在主目录文件夹后，直接跳至3.)
2. Windows系统在已安装git的情况下，点击鼠标右键并点击"Git Bash here"，弹出bash窗口；
3. 继续按顺序执行以下命令：
```
# testtest
$ git init  
$ git checkout -b backup  
$ git add .  
$ git commit -m "commit message"  
$ git remote set-url https://github.com/yourname/yourname.github.io.git
$ git push origin backup
```



