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