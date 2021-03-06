# rg

| 名                 | 曰                                                                                                                                             |
|--------------------|------------------------------------------------------------------------------------------------------------------------------------------------|
| `-h`               | 显示 ripgrep 的浓缩帮助输出。                                                                                                                  |
| `--help`           | 显示 ripgrep 的更长形式的帮助输出。(几乎是你在 ripgrep 的 man 页面里找到的，所以把它变成一个传呼机!)                                           |
| `-i/--ignore-case` | 当搜索模式时，忽略案例差异。那就是`rg -i fast`匹配`fast`，`fASt`，`FAST`等。                                                                   |
| `-S/--smart-case`  | 这类似于`--ignore-case`但如果模式包含大写字母，则禁用它自己。通常将此标志放入别名或配置文件中。                                                |
| `-w/--word-regexp` | 要求图案的所有匹配都被单词边界包围。也就是说，给出`pattern`， the `--word-regexp`标志会使 ripgrep 表现得像`pattern`实际上是`\b(?:pattern)\b`。 |
| `-c/--count`       | 报告总匹配行的计数。                                                                                                                           |
| `--files`          | 打印 ripgrip *将要*搜索的文件，但不要实际搜索它们。                                                                                            |
| `-a/--text`        | 搜索二进制文件，就好像它们是纯文本一样。                                                                                                       |
| `-z/--search-zip`  | 搜索压缩文件(gzip, bzip2, lzma, xz, lz4, brotli, zstd)。默认情况下这是禁用的。                                                                 |
| `-C/--context`     | 显示匹配周围的行。                                                                                                                             |
| `--sort path`      | 强制 ripgrep 将其输出按文件名排序。(这禁用并行性，所以它可能会慢一些。)                                                                        |
| `-L/--follow`      | 在递归搜索的同时，遵循符号链接。                                                                                                               |
| `-M/--max-columns` | 限制 ripgrip 打印的行的长度。                                                                                                                  |
| `--debug`          | 显示 ripgrip 的调试输出。这对于理解为什么在搜索中可以忽略特定文件，或者 ripgrep 正在从环境中加载何种配置非常有用。                             |