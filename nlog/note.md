## tex 基本语法

要了解 latex 的基本编程语法，enviroments 和 commands 这两个概念非常重要

命令 `\command[]{}`，方括号为可选参数，花括号为必选参数

环境 `\begin{}[]`，方括号为可选参数，花括号为必选参数

参考：[latex 命令语法](https://www.overleaf.com/learn/latex/Commands),
[latex 环境语法](https://www.overleaf.com/learn/latex/Commands)

## 常用宏包的使用

### 伪代码

参考：<https://zhuanlan.zhihu.com/p/166418214> (知乎-Algorithm2e 简明指南)

用伪代码写算法，常用的包`Algorithm2e`，支持中文，常用命令有：

![](assets/img/readme_2022-04-17-22-19-14.png)

如果你不想让你的伪代码叫做 'Algorithm 编号'， 可以使用 `\renewcommand{\algorithmcfname}{算法名}` 命令来修改。

### 插入图片

参考：<https://zhuanlan.zhihu.com/p/32925549> (知乎)

下面是相关代码：

```tex
%使用三个宏包
\usepackage{graphicx} %插入图片的宏包
\usepackage{float} %设置图片浮动位置的宏包
\usepackage{subfigure} %插入多图时用子图显示的宏包

\includegraphics[width=0.7\textwidth]{DV_demand} %插入图片，[]中设置图片大小，{}中是图片文件名
```

上面的`DV_demand`是指定文件名，可以看到没有后缀，所以如果你指定图片的当前目录有很多个同名不同格式的图片，这个时候就不知道latex会选择哪个格式的文件进行编译
