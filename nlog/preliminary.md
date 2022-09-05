## MathJax和katex

引擎，经常用于markdown中。

[wiki百科][1]中提到，mathjax只支持latex的用来描述数学符号的子集：

> Because MathJax is meant only for math display, whereas LaTeX is a document layout language, MathJax only supports the subset of LaTeX used to describe mathematical notation.

也提到了LaTeX是document layout language，但wiki中并没有document layout language的定义

[知乎][2]中提到：

> - VScode的Markdown preview enhanced（MPE）插件支持和 两类渲染引擎
>
> - Typora用的也是MathJax引擎

[1]:https://en.wikipedia.org/wiki/MathJax "mathjax wiki"
[2]:https://zhuanlan.zhihu.com/p/381263375 "Mathjax和katex"

## 相关概念

- 文学编程(literate programming)，第一个文学编程环境是 web

- latex 中涉及的文件格式有：`.tex`，`.bib`，`sty`，`bbl`等：

  - `bib`,`bbl`：写参考文献的文档
  - `sty`：包文件，通常使用`\usepackage`导入
  - `cls`：类文件，通过文档最前面的`\documentclass`命令导入

  参考：[latex 相关文件以及 cls 文件怎么写](https://zhuanlan.zhihu.com/p/77537952)

- .ins和.dtx文件，参考：<https://liam.page/2015/01/23/literate-programming-in-latex/>

## Kpathsea

a library to do path searching，参考：<https://tug.org/kpathsea/>
