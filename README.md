# 超强vim配置文件


### 简易安装方法：

打开终端，执行下面的命令就自动安装好了：

`curl -sSL https://raw.github.com/ma6174/vim/master/setup.sh | sh`

### 或者自己手动安装：(以ubuntu为例)

1. 安装vim `sudo apt-get install vim`
- 安装ctags：`sudo apt-get install ctags`
- 安装一些必备程序：`sudo apt-get install python-twisted xclip vim-gnome astyle python-setuptools`
- python代码格式化工具：`sudo easy_install -ZU autopep8`
- `sudo ln -s /usr/bin/ctags /usr/local/bin/ctags`
- clone配置文件：`cd ~/ && git clone git://github.com/ma6174/vim.git`
- `mv ~/vim ~/.vim`
- `mv ~/.vim/.vimrc ~/`
- clone bundle 程序：`git clone https://github.com/gmarik/vundle.git ~/.vim/bundle/vundle`
- 打开vim并执行bundle程序`:BundleInstall`
- 重新打开vim即可看到效果

### 了解更多vim使用的小技巧：

[tips.md](tips.md)

### 查看更新日志：

Note：
增加了scope搜索代码的功能:在代码顶级目录下执行scope . 会在tmp目录下得到检索信息，用于代码搜索
需要把bin/scope可执行文件放到PATH环境变量中，scope使用的快捷键:
    ctrl+i 向前跳到前几次光标位置
    ctrl+o 向后跳到后几次光标位置
    Esc + e 相当于egrep 搜索
    Esc + d  查找本函数调用的函数
    Esc + c   查找调用本函数的函数
    Esc + g   查找定义的地方
安装步骤：
1.原项目正常安装
2.添加scope到PATH环境变量中即可

本项目是在https://github.com/itscamp/vim.git基础上修改得到的，感谢原作者！
