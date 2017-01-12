---
title: vim的简单配置
date: 2017-01-08 07:14:03
tags: linux
categories: 技术
---
简单配置

输入命令：
```
sudo vim /etc/vim/vimrc
```
<!-- more -->
在.vimrc文件中输入如下文本:

```
set tabstop=4         #Tabstop:表示一个 tab 显示出来是多少个空格的长度,默认 8。 
set softtabstop=4     #Softtabstop:表示在编辑模式的时候按退格键的时候退回缩进的长度,当使用 expandtab 时特别有用
set shiftwidth=4      #Shiftwidth:表示每一级缩进的长度,一般设置成跟    softtabstop 一样。 当设置成 expandtab 时,缩进用空格来表示
set noexpandtab       #noexpandtab 则是用制表符表示一个缩进。 
set nu                #nu:表示显示行号。 
set autoindent        #Autoindent:表示自动缩进。 
set cindent           #Cindent:是特别针对C语言自动缩进。
```

# 一、配置

 如果你需要配置vim，只需在Home目录创建一个~/.vimrc文件即可以配置vim了，可以参考我的vimrc配置文件。由于我需要安装插件，并且将需要安装的插件列表分离到另外一个文件~/.vimrc.bundles，这个文件也是存放在Home目录，文件内容可以参考vimrc.bundles。若想加载~/.vimrc.bundles文件，必须在~/.vimrc文件加入以下代码片段：
``` 
if filereadable(expand("~/.vimrc.bundles"))
source ~/.vimrc.bundles
endif
```

# 二、插件

插件管理工具vunble

vundle是vim的插件管理工具，它能够搜索、安装、更新和移除vim插件，再也不需要手动管理vim插件。
在Home目录创建~/.vim目录和.vimrc文件（可复制我的vimrc文件）

## 安装vundle

```
git clone https://github.com/gmarik/vundle.git ~/.vim/bundle/vundle
```

## 在.vimrc配置文件中添加vundle支持

```
filetype off
set rtp+=~/.vim/bundle/vundle/
call vundle#rc()
```

但实际上我是添加一个~/.vimrc.bundles文件来保存所有插件的配置，必须在~/.vimrc文件加入以下代码片段：

```
if filereadable(expand("~/.vimrc.bundles"))
source ~/.vimrc.bundles
endif
```

而~/.vimrc.bundles文件内容必须包含：

```
filetype off
set rtp+=~/.vim/bundle/vundle/
call vundle#rc()
```

你可以复制到我~/.vimrc.bundles文件到Home目录。

## 安装插件

bundle分为三类，比较常用就是第二种：
在Github vim-scripts 用户下的repos,只需要写出repos名称
在Github其他用户下的repos, 需要写出”用户名/repos名”
不在Github上的插件，需要写出git全路径

将安装的插件在~/.vimrc配置，但是我是将插件配置信息放在~/.vimrc.bundles：

```
" Define bundles via Github repos
Bundle 'christoomey/vim-run-interactive'
Bundle 'Valloric/YouCompleteMe'
Bundle 'croaky/vim-colors-github'
Bundle 'danro/rename.vim'
Bundle 'majutsushi/tagbar'
Bundle 'kchmck/vim-coffee-script'
Bundle 'kien/ctrlp.vim'
Bundle 'pbrisbin/vim-mkdir'
Bundle 'scrooloose/syntastic'
Bundle 'slim-template/vim-slim'
Bundle 'thoughtbot/vim-rspec'
Bundle 'tpope/vim-bundler'
Bundle 'tpope/vim-endwise'
Bundle 'tpope/vim-fugitive'
Bundle 'tpope/vim-rails'
Bundle 'tpope/vim-surround'
Bundle 'vim-ruby/vim-ruby'
Bundle 'vim-scripts/ctags.vim'
Bundle 'vim-scripts/matchit.zip'
Bundle 'vim-scripts/tComment'
Bundle "mattn/emmet-vim"
Bundle "scrooloose/nerdtree"
Bundle "Lokaltog/vim-powerline"
Bundle "godlygeek/tabular"
Bundle "msanders/snipmate.vim"
Bundle "jelera/vim-javascript-syntax"
Bundle "altercation/vim-colors-solarized"
Bundle "othree/html5.vim"
Bundle "xsbeats/vim-blade"
Bundle "Raimondi/delimitMate"
Bundle "groenewege/vim-less"
Bundle "evanmiller/nginx-vim-syntax"
Bundle "Lokaltog/vim-easymotion"
Bundle "tomasr/molokai"
Bundle "klen/python-mode"
```
打开vim，运行```:BundleInstall```或在shell中直接运行```vim +BundleInstall +qall```



