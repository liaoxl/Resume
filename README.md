使用moderncv打造个人简历
=======


用latex制作cv的想法源于这个[开源项目](https://github.com/zellux/resume)，我把它下载下来，在自己机器上安装了Texlive(系统是Fedora 17)，发现编译中文简历有问题，似乎是编码的问题。我大概看了下这位作者所使用的模板是[moderncv](http://www.ctan.org/tex-archive/macros/latex/contrib/moderncv)的模板，所以下载下来自己按照模板写了，并创建了自己的[简历开源项目](https://github.com/liaoxl/Resume)

如果总结起来的话，其步骤大概如下：

1. 配置Texlive环境，我当时直接下载的ISO文件（直接`yum`安装的，因为源里的版本比较旧，对中文支持不好），在我校的[开源站点](http://mirror.hust.edu.cn/CTAN/systems/texlive/)，然后用这个命令挂载`mount -o loop -t iso9660 /home/moondark/Downloads/texlive2013-20130530.iso /mnt/vcdrom/`，当然前提你得在`/mnt/`目录下创建`vcdrom/`这个目录;

2. 下载[moderncv](http://www.ctan.org/tex-archive/macros/latex/contrib/moderncv)的格式文件;

3. 仿造[modercv](http://www.ctan.org/tex-archive/macros/latex/contrib/moderncv)上面的examples来书写自己的简历;

4. 我用`pdflatex`命令编译的，好像用`xelatex`命令也可以，具体区别我也不甚清楚


简历效果
====

[中文简历](http://files.cnblogs.com/moondark/XiangliLiao-zh.pdf)

[英文简历](http://files.cnblogs.com/moondark/XiangliLiao-en.pdf)

---

moderncv -- a modern curriculum vitae class

Moderncv provides a documentclass for typesetting curriculum vitaes in various
styles. It aims to be both straightforward to use and customizable, providing
four ready-made styles (classic, casual, banking and oldstyle) and allows you to
define your own style by easily modifying colors, fonts, etc.

Most commands are defined in such a way that arguments are optional.

Until a decent manual is written, you can always look in the "examples"
directory for some examples. Documents can be compiled into dvi, ps or pdf.


Author: Xavier Danaux <xdanaux@gmail.com>
Licence: The LaTeX Project Public Li­cense, version 1.3c
