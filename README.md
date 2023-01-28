# MyBookdownArticleTemplete
一个基于bookdown和ctexart文档类的R-markdown模板。建议用来输出`PDF`文件。

# 文件介绍

## 编译前

- `index.Rmd`主文件，在此文件中编写内容

- `mybib.bib`参考文献库
- `preamble.tex`用于LaTex编译的导言区
- `_bookdown.yml`一些bookdown的全局设置
- `_output.yml`输出设置
- `_header.html`输出HTML的一些额外设置
- `Modified_Record.txt`对原模板的修正记录
- `figures`准备自行插入的图片文件夹

## 编译后新增

- `_book`编译得到的主要内容。其中`_main.pdf`文件就是是我们需要的。

- `_bookdown_files`储存图片等结果。

- `_main-tikzDictionary`调用`tike`画图的一个中间结果

# 编译方式与编码

- 编码默认为UTF-8。

- RStudio右上角的`bulid`按钮编译。

- 可以将`_book`中的`_main.tex`，主目录中的`mybib.bib`和`figures`文件夹移动到`_bookdown_files`中，打开`.tex`文件进行编辑和编译。

- TeX内部需编译5次。顺序为XeLaTeX - makeindex - biber - XeLaTeX - XeLaTeX 。建议使用TexLive2022+TexStudio运行。

# 参考文献

本模板是基于北京大学李东风老师的模板修改得到。具体为[原模板](https://www.math.pku.edu.cn/teachers/lidf/docs/Rbook/html/_Rbook/bookdown-template-v0-6.zip)中的`Books/CArticle`。

益辉大大：[bookdown: Authoring Books and Technical Documents with R Markdown](https://bookdown.org/yihui/bookdown/)

李东风老师：[R语言教程](https://www.math.pku.edu.cn/teachers/lidf/docs/Rbook/html/_Rbook/bookdown.html)

汤银才老师：[Bookdown中文书稿写作手册](https://tangyc8866.github.io/bookdown_tutorial/)

高春辉，王祎帆，闫求识，庄亮亮，杨晓龙等：[R Markdown 指南](https://cosname.github.io/rmarkdown-guide/)

[CTeX宏包说明文档](https://mirrors.tuna.tsinghua.edu.cn/CTAN/language/chinese/ctex/ctex.pdf)

[一份（不太）简短的 LaTeX 2ε 介绍](https://mirrors.tuna.tsinghua.edu.cn/CTAN/info/lshort/chinese/lshort-zh-cn.pdf)

在此一并表示感谢！

# 更新信息

- **v1.0**  *JieYin-NENU on Jan,28,2023*
