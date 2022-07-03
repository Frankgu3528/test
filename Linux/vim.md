# vim的使用

关于vim，江湖上流传着它的传说，有人说它是神的编辑器，有人说它是编辑器的神，也有人说他就是垃圾。不管怎样，安装好vim开始折腾吧。

```bash 
sudo apt-install vim
```

## 编写第一个程序


#### C++

重点介绍一下怎么写在Linux下写出一个hello world程序。

c++有很多编译器可供选择，大名鼎鼎的gcc/g++，另外还有clang，msvc等。一般用g++来编译c++程序，gcc理论上应该也可以，但实际使用下似乎有点问题。

Linux似乎预装了gcc编译器，但g++似乎要手动下。在Ubuntu下似乎用apt就能安装。

**做好了准备工作，那么我们开始吧**！

首先在vim下新建一个文件

```
vim hello.cpp
```

进入vim后是普通的模式，按i进入插入模式进行编辑，写一个简单的cpp程序。

```
#include <iostream>
using namespace std;
int main(){
        cout<<"hello world"<<endl;
        return 0;
}                           
```

按esc退出插入模式，按：进入尾行模式，按wq进行保存并退出。

这样就回到了终端中，可以输入ls查看文件目录，发现多了hello.cpp文件。

接着用g++编译：

```
g++ hello.cpp
```

如果没有报错就说明没有问题。在输入ls命令，可以看到目录下多了a.out文件，输入

```
./a.out
```

执行文件，即可出现：

```
hello world
```

#### Python

Ubuntu内置了Python。命令行输入

```
python3
```

可查看安装的版本。（Ubuntu22.04似乎内置了Python 3.10.4）

类似C++，我们可以

```
vim hello.py
# 写你的程序
python3 hello.py
./a.out
```

来得到输出。

## 更上一层楼

vim的魅力远不在此。通过修改配置文件，你可以将vim定制成任何你想要的样子，以及按你的习惯修改各种操作, 这可以让你远离鼠标。

此处不在一一介绍，不过以下是一些可以折腾的地方。

1. 修改键位。(强烈建议把大写锁定键映射成esc，这个键占了键盘的黄金键位但用处很少)
2. 熟悉vim的几种模式
3. 熟悉vim的快捷键，比如可以通过shift+a快速调到行的末尾。
4. ~~美化vim~~（逃）
