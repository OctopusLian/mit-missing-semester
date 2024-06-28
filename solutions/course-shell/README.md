# Solution-课程概览与 shell  

1.在 /tmp 下新建一个名为 missing 的文件夹。  

```shell
mkdir missing
```

2.用 man 查看程序 touch 的使用手册。  

```shell
man touch
```

3.用 touch 在 missing 文件夹中新建一个叫 semester 的文件。  

```shell
touch semester
```

4.将以下内容一行一行地写入 semester 文件。  

5.尝试执行这个文件。  

```shell
./semester
```

6.查看 chmod 的手册。  

```shell
man chmod
```

7.使用 chmod 命令改变权限，使 ./semester 能够成功执行，不要使用 sh semester 来执行该程序。  

```shell
chmod 777 semester
```

8.使用 | 和 > ，将 semester 文件输出的最后更改日期信息，写入主目录下的 last-modified.txt 的文件中。  

9.写一段命令来从 /sys 中获取笔记本的电量信息，或者台式机 CPU 的温度。  