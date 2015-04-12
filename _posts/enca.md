title: "enca"
date: 2015-04-12 20:03:35
tags:
---

1. 安装
2. 查看当前文件编码
`enca -L zh_CN ip.txt`     Simplified Chinese National Standard; GB2312     Surrounded by/intermixed with non-text data  　　
3. 转换命令格式如下  　　
`$enca -L 当前语言 -x 目标编码 文件名`

-----
例如要把当前目录下的所有文件都转成utf-8  　　
`enca -L zh_CN -x utf-8 *`
检查文件的编码
`enca -L zh_CN file`
将文件编码转换为"UTF-8"编码
`enca -L zh_CN -x UTF-8 file`
如果不想覆盖原文件可以这样
`enca -L zh_CN -x UTF-8 < file1 > file2`
