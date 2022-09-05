## 部署

### 编译

一般使用`pdflatex`, `lualatex`，`latex`等带有`latex`字样的编译器来编译，编译后即可生成 pdf 文件。

此外还有`tex`，`luatex`等编译器，这些只能编译纯tex源文件

### 下载和安装

主要介绍archlinux环境，建议使用yay安装(可以安装texlive-full，几乎包括了latex的一切)，使用pacman安装还需要考虑额外包安装的问题

#### 使用yay安装texlive-full

使用这种方式安装好tex后，基本不需要安装额外的tex包

#### 使用pacman

##### 安装tlmgr

arch下的install prefix为`~/texmf`

- 创建alias，`alias tlmgr="$TEXMFDIST/scripts/texlive/tlmgr.pl --usermode"`
  - 查询TEXMFDIST在archlinux中的默认值，定义环境变量TEXMFDIST

- 修改`/usr/share/texmf-dist/scripts/texlive/tlmgr.pl`中的`$Master = "$Master/../..";`
- 初始化tlmgr
- 添加镜像
- 安装CTAN packages

具体参考：<https://wiki.archlinux.org/title/TeX_Live#tlmgr>

##### 安装额外的包

`tlmgr install <package1> <package2> ...`

`tlmgr remove <package1> <package2> ...`

具体参考：<https://en.wikibooks.org/wiki/LaTeX/Installing_Extra_Packages>

##### 安装包的路径问题

> used always to tell you to put your files “where LaTeX can find them”; this was always unhelpful

- 哪些路径(tree)latex会搜寻
- 不同类型的文件应该tree路径的哪个位置

参考：<https://texfaq.org/FAQ-inst-wlcf> k what tree to use k where in the tree to put the files

## preliminary

## 经验

## FAQ

### xmind中的latex公式如何换行

参考：<https://www.xmind.cn/blog/cn/how-to-use-latex-in-xmind/>

### 对齐多组和多行公式

参考：<https://www.xmind.cn/blog/cn/how-to-use-latex-in-xmind/> k 如果你想对齐多组公式

### 为什么编译不通过

使用某些包后，pdflatex就会编译不通过(具体原因不清楚)，请使用lualatex进行编译

## 推荐参考资料

### 官方文档

<https://www.latex-project.org/help/documentation/> k A short introduction to LaTeX kp LaTeX2e for authors

### 经验学习

<https://www.xmind.app/faq/question/equation/#chemical-equation> xmind关于latex公式的文档(xmind使用MathJax)

## by the way

### md使用`<script>`标签引入MathJax

参考：<https://www.cnblogs.com/Neo007/p/7711499.html>
