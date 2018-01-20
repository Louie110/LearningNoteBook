
参考资料：[使用Markdown + Pandoc + LaTex + Beamer制作幻灯片](http://www.cnblogs.com/aquastone/p/markdown_slide.html)

# 基本过程和工具
mardown 制作幻灯片的流程一般是：先用 markdown 写文本文件，然后使用工具转化为 html 或 pdf 等格式。 这个过程如有必要，可修改 css 或 tex 模板。 用到的工具有：
- 任何文本编辑器：用于编辑 markdown 源文件
- pandoc：将 markdown 转换成其他格式（本文主要介绍 pdf）的工具
- latex：pandoc 将 markdown 转换成 pdf 时，需要用到 latex 引擎。如果要支持中文，可以装 xelatex
- beamer：latex 下制作幻灯片的工具包

当然，直接用 latex+beamer 就可以制作幻灯片，但是需要写 tex 源文件，比较麻烦而且可读性不如 markdown。 所以我采用 markdown 写内容，tex做模板的方式。

# 一个基本的幻灯片
## 编辑 markdown 源文件
pandoc 将 markdown 的一级标题视为幻灯片组，将二级标题视为幻灯片标题，二级标题下的内容放在一张幻灯片里。 不过，如果某个一级标题下没有二级标题，那么pandoc将把一级标题视为幻灯片标题，将这个一级标题下的内容放在一张幻灯片里， 二级标题显示为子框。
在任何时候，用 `---------` 都可以产生一张新幻灯片。
pandoc对 markdown有个扩展，在前面加上三行以 `%` 开头的内容，分别是标题、作者和日期。
例子如下

```md
% Title
% auther
% date

# This is a group

## This is title 1

  This is first slide

  - item 1
  - item 2

## This is tile 2

  This is second slide

-------------

  This is third slide
```

## 转换为 pdf
将上述代码保存为 exam1.md，运行
```sh
pandoc -t beamer -o exam1.pdf exam1.md
```
即可生成 pdf。

## pandoc 对 markdown 的扩展
pandoc 出了支持标准的 markdown 语法，还作了一些很实用的扩展，上面的标题、作者和日期就是。 此外比较实用的还有表格、公式等。详见 [pandoc的文档](http://pandoc.org/MANUAL.html)。

## 中文支持
要正常显示中文，需要注意两点：
- 使用 xelatex 引擎
- 在模板文件中正确配置

首先导出 pandoc 的 beamer 默认配置
```sh
pandoc -D beamer > beamer-template.tex
```

在 `\ifxetex` 后面加入对中文的支持
```tex
\usepackage{xeCJK}                 % 设置中英文字体
\setCJKmainfont{WenQuanYi Micro Hei} % 中文字体
\setmainfont{Arial}                % 英文字体
\setromanfont{Courier New}
\setmonofont{Courier New}
\linespread{1.2}\selectfont        % 行距
\XeTeXlinebreaklocale "zh"         % 中文自动换行
\XeTeXlinebreakskip = 0pt plus 1pt % 字之间加0pt至1pt间距
\parindent 0em                     % 段缩进
\setlength{\parskip}{20pt}         % 段间距
```
编译时使用命令
```sh
pandoc -t beamer --latex-engine=xelatex --template=beamer-template.tex xx.md -o xx.pdf
```
