# [玩转Mac常用命令、zsh等技巧，挖掘Mac潜力](https://www.jianshu.com/p/28de342f5ecc)
## archey:
## ccat:
## tree 命令安装:
功能：
将文件以目录树的形式展开，方便查看文件，非常实用的一个插件。
Mac 系统本身不自带 tree命令，需要安装：
1. 首先，进入目录：
```bash
cd $home
```
2. 使用vim 命令创建一个.bashrc文件，并在里面添加如下一行代码：
```bash
vi .bashrc
alias tree="find . -print | sed -e 's;[^/]*/;|____;g;s;____|; |;g'"
```
立即生效
```bash
source .bashrc
```
查看文件树结构
命令行执行：
```bash
tree
```
##dict
>用于翻译的命令行工具，基于python

## [MAC下安装iterm2+oh my zsh超详细过程](https://blog.csdn.net/qq_32958797/article/details/97307977) 
- 2020-06-19-23:49
- ps:因为自己看到很多人说oh my zsh 还有终端还是不太会使用所以找到这个网址学习