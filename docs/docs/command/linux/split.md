---
title: split
description: [hakcettyu's cheetsheet]
---

> description: [hakcettyu's cheetsheet]

- split -l {{1}} {{filename}}

  分割一个文件每次分割 10 行，除了最后一次分割

- split -n {{5}} {{filename}} 
 
 将一个文件拆分为 5 个文件。文件被拆分，这样每个拆分的大小相同（除了最后一个拆分）。

- 拆分一个文件，每个拆分中有 512 个字节（除了最后一个拆分；使用 512k 表示千字节，512m 表示兆字节）。

- split -C {{512}} {{filename}}

 拆分一个文件，每个拆分最多 512 个字节，不换行

- split -b 20M foo.mv

    尺寸单位缩写为 K，M，G，T，P，E，Z，Y（1024 的幂）或者 KB，MB，GB 等等（1000 的幂）
    

