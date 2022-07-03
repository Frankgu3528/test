# lec1 shell

## 单词

| 单词        | 意义                     |
| ----------- | ------------------------ |
| slash       | 斜杠                     |
| directory   | 目录（可以理解成文件夹） |
| repectively | 分别得，各自得           |

![image-20220620123114495](C:\Users\阿漆\AppData\Roaming\Typora\typora-user-images\image-20220620123114495.png)

## 知识

| 命令 | 作用 |
| ---- | ---- |
|    ls  | 列出这个文件夹下的东西 |
| pwd | 告诉我现在在哪里 |
| ls -l | 列出更完整的信息 |

In a path, `.` refers to the current directory, and `..` to its parent directory:

```
missing:~$ ls -l /home
drwxr-xr-x 1 missing  users  4096 Jun 15  2019 missing
```

First, the `d` at the beginning of the line tells us that `missing` is a directory.
### Linking Programs

