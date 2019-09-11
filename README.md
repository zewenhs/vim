# 超强vim配置文件

[![Build Status](https://travis-ci.org/ma6174/vim.png?branch=master)](https://travis-ci.org/ma6174/vim)

### 运行截图

![screenshot.png](screenshot.png)

### 特点
 我的vim配置主要有以下优点：

1. 按F5可以直接编译并执行C、C++、java代码以及执行shell脚本，按“F8”可进行C、C++代码的调试

2. 自动插入文件头 ，新建C、C++源文件时自动插入表头：包括文件名、作者、联系方式、建立时间等，读者可根据需求自行更改

3. 映射“Ctrl + A”为全选并复制快捷键，方便复制代码

4. 按“F2”可以直接消除代码中的空行

5. “F3”可列出当前目录文件，打开树状文件目录

6. 支持鼠标选择、方向键移动

7. 代码高亮，自动缩进，显示行号，显示状态行

8. 按“Ctrl + P”可自动补全

9. []、{}、()、""、' '等都自动补全

10. 其他功能读者可以研究`.vimrc`文件


### 简易安装方法：

打开终端，执行下面的命令就自动安装好了：

`wget -qO- https://raw.github.com/ma6174/vim/master/setup.sh | sh -x`

### 或者自己手动安装：(以ubuntu为例)

1. 安装vim `sudo apt-get install vim`
- 安装ctags：`sudo apt-get install ctags`
- 安装一些必备程序：`sudo apt-get install xclip vim-gnome astyle python-setuptools`
- python代码格式化工具：`sudo easy_install -ZU autopep8`
- `sudo ln -s /usr/bin/ctags /usr/local/bin/ctags`
- clone配置文件：`cd ~/ && git clone git://github.com/ma6174/vim.git`
- `mv ~/vim ~/.vim`
- `mv ~/.vim/.vimrc ~/`
- clone bundle 程序：`git clone https://github.com/gmarik/vundle.git ~/.vim/bundle/vundle`
B
- 打开vim并执行bundle程序`:PluginInstall`
- 重新打开vim即可看到效果

### YouCompleteMe 的安装配置
[ubuntu下vim 安装插件管理工具Vundle和自动补全插件YouCompleteMe](https://blog.csdn.net/m0_37624499/article/details/89526701)  
在 ~/.vimrc 文件中加入如下命令实现 F7 跳转到函数定义处：
`nnoremap <F7> :YcmCompleter GoToDefinitionElseDeclaration<CR> `

### vim-airline 的安装配置
[安装配置 Vim-airline](https://www.jianshu.com/p/f4ff48c196af)

### 了解更多vim使用的小技巧：

[tips.md](tips.md)

### 查看更新日志：

[`update_log.md`](update_log.md)
