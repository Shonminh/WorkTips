- rm -rf -f 忽略不存在的文件，从不给出提示。-r -R 删除子目录


- cat /etc/shells 查看当前shell种类 chsh -l
- chsh -s /bin/zsh 修改登录的shell
- touch file 用来创建文件，如果存在，则该命令会更新时间戳。ls -l
- grep命令用来显示文件和输入流中和参数匹配的行。
- ctrl + U 回退当前命令，不换行
- ctrl + C 终止当前命令，换行
- mkdir -p 创建中间文件 如：mkdir -p /path/with/many/layer 则会创建中间层的目录
- mkdir -m 制作文件夹的权限
- diff file1 file2 比较两者的区别，diff -u 格式更加易读

###在写shell时的文本编辑操作
*注:*在终端时极为使用，效率！

1. Ctrl+B 左移光标
2. Ctrl+F 右移光标
3. Ctrl+P 查看上一条命令
4. Ctrl+N 查看下一条命令
5. Ctrl+A 光标至行首
6. Ctrl+E 光标至行尾
7. Ctrl+W 删除前一个词
8. Ctrl+U 删除从光标至行首的内容


*注：*这是BSD风格，ps支持三种风格，导致显示有些区别

1.   UNIX options, which may be grouped and must be preceeded by a dash.
2.   BSD options, which may be grouped and must not be used with a dash.
3.   GNU long options, which are preceeded by two dashes.

- ps x 显示当期用户的所有进程
- ps ax 显示当前系统运行的所有进程，包括其他用户的进程
- ps u 显示更详细的进程信息
- ps w 显示命令的全名
