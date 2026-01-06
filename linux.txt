
https://www.runoob.com/linux/linux-tutorial.html
ls  # 输出当前目录下的文件名称
ls -l  # 输出当前目录下的文件的信息 (long listing)
more <file> # 查看文件
mkdir <dir>  # 创建目录
mv <file> <dir>  # 移动文件
mv <file-name1> <file-name2>  # 重命名文件
cd <dir>  # 切换工作目录
cd ..  # 切换到父目录
cd  # 切换到自己的home目录（也可用cd ~）
pwd  # 输出工作目录
cp <file> <dir>  # 复制文件
rm <file>  # 删除文件
rmdir <dir>  # 删除空目录
chmod o+x <file>  # 修改权限：给其他用户执行权 (change mode)
chmod ugo-rwx <file>  # 把所有权限关掉
groups  # 查看自己所在的组
man <command> # 参考手册 (manual)
man man  # 查找指令
man -k 字符  # 查找指令
finger <user-name>  # 查找用户信息
find <dir> -name "xxx*"  # 查找 (如果要用通配符，就要加引号，否则可以不用)
cat <file1> <file2>  # 拼接文件内容（也可以同时拼接多个文件）
cat f1 f2 > f3  # 将输出发送到文件f3，可用>或>>。若f3已存在，则它原本的内容会被覆盖。若你只是想把内容加到原有内容后面，用>>，不要用>
权限码：第一位：- 表示文件；d 表示目录；后面接三组字符（所有者u，组g，其他人o），每组有3个字符
-rw-r--r-- keeper prim 547 9:31 ch
权限码 用户名 组名 文件大小 最后修改时间 文件名
rwx =读，写，执行（只有当文件是程序时才可以有执行权限）对应位置如果是-表示没有该权限
通配符(wildcards) *可匹配任意数目的字符（0个也可以）?只匹配1个字符

当你登入Linux系统时，你自动地位于自己的home目录。
. 表示当前目录
.. 表示父目录
~ 表示自己的home目录
~用户名 可指定其他用户的home目录。当~后面接/以外的东西，Linux会假定你在指其他用户的home目录
