[TOC]

### 安装方法

```
git clone --recursive https://github.com/zkdfbb/vim.git ~/.vim && (echo | vim +BundleInstall +qall)
```

### 插件说明

#### Vundle

管理第三方插件，初始化

```
vim +BundleInstall! +BundleClean +q
:BundleInstall    #安装
:BundleUpdate     #升级
```

#### vim-plug

用于管理第三方插件，支持并发安装，用法和Vundle类似

https://github.com/junegunn/vim-plug

#### vim-jsbeautify

javascript排版插件。使用用法：

```
:call JsBeautify()
```

#### tagbar

需要先安装ctags

```
sudo apt-get install ctags
```

大纲式导航，包含类/方法/变量等, 可以选中快速跳转到目标位置。使用方法：

```
:TagbarToggle
```

快捷键：`F9`

#### nerdtree

显示树形目录。使用方法：

```
:NERDTreeToggle
```

快捷键：`F8`

#### emmet-vim

用于快速编写html，如输入缩略词组div#page>ul>li*3然后按Ctrl+y+,即可展开成html代码

#### YouCompleteMe

自动补全插件，升级&安装方法：

```
git submodule update --init --recursive
./install.py
```

#### ale

代码异步检测插件，要求vim版本 >= 8.0

#### python-mode

要求python使用--enable-shared参数编译。

用于python开发环境，如自动格式化

```
:PymodeLintAuto
```

快捷键：`Ctrl+m`

#### vim-powerline

vim状态栏美化插件

#### vim-airline

vim状态栏美化插件

#### vim-colorschemes

vim字体颜色美化插件

#### tabular

自动对齐代码，选中代码块，如原代码：

```
one = 1
two = 2
three = 3
four = 4
```

选中之后输入:Tab /= ，会格式化成

```
one   = 1
two   = 2
three = 3
four  = 4
```

#### 语法高亮插件

1. vim-markdown
2. pig.vim
3. vim-scala
4. nginx.vim

#### neocomplete     补全插件

需要vim添加lua支持

```
sudo apt-get install ncurses-dev python-dev lua5.1 liblua5.1-dev -y
```

#### xptemplate    重复代码插件

在insert模式下输入片段代码的名字(如switch)，然后按<C-\>(即Ctrl+\)

然后按tab、shift tab前后更改高亮显示的内容


#### incsearch.vim

增强vim的搜索功能

#### vim-signify

vim版本控制，同时支持Git 和 Svn，高亮当前修改

### 快捷键

1. F1:帮助(默认)
2. F2:切换窗口
3. F3:去行尾空格(普通模式)
3. F4:去空行(普通模式)
4. F5:编译运行
6. F6:调试运行
7. F7:粘贴模式
8. F8:打开/关闭NERDRree
9. F9:打开/关闭Tagbar
10. F10:Python代码格式化
11. F11:最大化(默认)
12. F12:自动插入文件头部声明
13. Ctrl+m: 代码格式化
14. Ctrl+l: 打开/关闭语法检查
15. Ctrl+k: 跳转到上一个语法错误位置
14. Ctrl+j: 跳转到下一个语法错误位置
16. Ctrl+\: 跳转到函数定义处
17. Ctrl+b: 向上翻一页
18. Ctrl+f: 向下翻一页
19. b: 光标向前移动一个单词
20. w: 光标向后移动一个单词
21. ,b: 插入/删除python断点
22. :wq 保存退出, :qq 直接退出，:w!! 强制写入

### VIM技巧

[Vim编程——配置与技巧](http://linux-wiki.cn/wiki/%E7%94%A8Vim%E7%BC%96%E7%A8%8B%E2%80%94%E2%80%94%E9%85%8D%E7%BD%AE%E4%B8%8E%E6%8A%80%E5%B7%A7)

