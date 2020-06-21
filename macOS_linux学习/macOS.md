## [玩转Mac常用命令、zsh等技巧，挖掘Mac潜力](https://www.jianshu.com/p/28de342f5ecc)

____

## archey:

____

## ccat:

____

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
____

## dict

用于翻译的命令行工具，基于python

____

## [MAC下安装iterm2+oh my zsh超详细过程](https://blog.csdn.net/qq_32958797/article/details/97307977) 

- 2020-06-19-23:49
- ps:因为自己看到很多人说oh my zsh 还有终端还是不太会使用所以找到这个网址学习

____

## mac安装软件允许任何来源(sudo spctl --master-disable)

解决问题办法：

```bash
系统偏好设置 -> 安全性与隐私 -> 通用 -> 选择“任何来源”
```

“通用”里有时没有“任何来源”这个选项：

```bash
#显示"任何来源"选项在控制台中执行：

sudo spctl --master-disable

#不显示"任何来源"选项（macOS 10.12默认为不显示）在控制台中执行：

sudo spctl --master-enable

```

使用下载的破解软件：

```bash
xattr -r -d com.apple.quarantine <path>
```
____

## [Mac环境下VSCode配置python3](https://www.jianshu.com/p/354377ade444)