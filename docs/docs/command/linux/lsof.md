---
title: lsof
description: [hakcettyu's cheetsheet]
---

> description: [hakcettyu's cheetsheet]

- lsof -i :${port}  `列出谁在使用某个端口`
- lsof -p 11968 `通过某个进程号显示该进程打开的文件`
- lsof -i `列出所有的网络连接`
