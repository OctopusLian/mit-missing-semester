# Solution-Shell 工具和脚本  

1.阅读 man ls ，然后使用ls 命令进行如下操作  

```shell
# 所有文件（包括隐藏文件）  
ls -all   
total 8
drwxr-xr-x  3 neozhang  staff   96 Jun 27 15:54 .
drwxr-xr-x  7 neozhang  staff  224 Jun 27 15:50 ..
-rw-r--r--  1 neozhang  staff  306 Jun 27 15:54 README.md


# 文件打印以人类可以理解的格式输出 (例如，使用454M 而不是 454279954)
ls -all -h
total 8
drwxr-xr-x  3 neozhang  staff    96B Jun 27 15:55 .
drwxr-xr-x  7 neozhang  staff   224B Jun 27 15:50 ..
-rw-r--r--  1 neozhang  staff   425B Jun 27 15:55 README.md

# 文件以最近访问顺序排序
ls -all -t
total 8
drwxr-xr-x  3 neozhang  staff   96 Jun 27 15:56 .
-rw-r--r--  1 neozhang  staff  646 Jun 27 15:56 README.md
drwxr-xr-x  7 neozhang  staff  224 Jun 27 15:50 ..

# 以彩色文本显示输出结果

```

2.编写两个bash函数 marco 和 polo 执行下面的操作。 
每当你执行 marco 时，当前的工作目录应当以某种形式保存，当执行 polo 时，无论现在处在什么目录下，都应当 cd 回到当时执行 marco 的目录。 
为了方便debug，你可以把代码写在单独的文件 marco.sh 中，并通过 source marco.sh命令，（重新）加载函数。通过source 来加载函数，随后可以在 bash 中直接使用。