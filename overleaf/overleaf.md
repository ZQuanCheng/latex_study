
### 网址、账户

>
> https://www.overleaf.com/
>
> https://cn.overleaf.com/project
>
> 账户：google账号
>
> 




### 入门教程

> 
> bilibili：https://www.bilibili.com/video/BV1aN4y1K7qy
>
> 飞书云文档：https://xyfamily.feishu.cn/docx/MuhFdGc1lovo84xoq6pcScTSnbb
>
> Overleaf 帮助文档（强烈推荐）https://www.overleaf.com/learn
>
> LaTeX Cheatsheet 速查手册 `.\material\LaTeX Cheatsheet.pdf`
>
> 




#### LaTeX 从入门到够用（1）为什么应该用它写论文

> 
> <font color="gree"> 1. 内容和格式完全隔离  </font>
>
> 
> <font color="gree"> 2. 数学公式使用纯文本方式撰写  </font>
>
> 
> <font color="gree"> 3. 引用和修改参考文献很方便  </font>
>




#### LaTeX 从入门到够用（2）Overleaf 的使用

> 
> 客户端下载：https://www.latex-project.org/get/
> 
> 但是不建议本地部署，对新手不友好，而且有了`overleaf`没必要
> 
> 
> <font color="pink">（1）如何获取模板 </font>
> 
> > 中国科学院大学模板（非官方）：https://www.overleaf.com/latex/templates/ucasthesis/ktbzrphwzfjb
> > 
> > 清华大学模板：https://www.overleaf.com/latex/templates/thuthesis-tsinghua-university-thesis-latex-template/cfwgcxtvkbsx
> > 
> > <div align=center>
> > <img src="./images/overleaf_1.png"  style="zoom:100%"/>
> > <img src="./images/overleaf_2.png"  style="zoom:100%"/>
> > <img src="./images/overleaf_3.png"  style="zoom:100%"/>
> > </div> 
> > 
> > 点击`Open as Template`，默认把此模板复制到账号中
> > 
> > <div align=center>
> > <img src="./images/overleaf_4.png"  style="zoom:100%"/>
> > </div> 
> > 
> 
> 
> <font color="pink">（2）页面结构 </font>
> 
> > 左上角：文件结构树
> > 
> > 左下角：文章层级结构、大纲
> > 
> > 中间：纯文本
> > 
> > 右侧：编译结果、错误语句
> > 
> > <div align=center>
> > <img src="./images/overleaf_5.png"  style="zoom:100%"/>
> > <img src="./images/overleaf_6.png"  style="zoom:100%"/>
> > </div> 
> > 
> > 
> 
> 
> <font color="pink">（3）在模板基础上撰写 </font>
> 
> > 文件结构树大部分是设置文章样式，需要修改的极少
> > 
> > 我们只需要在 `data、figures、ref` 文件夹中添加内容就行
> > 
> > <div align=center>
> > <img src="./images/overleaf_7.png"  style="zoom:100%"/>
> > </div> 
> > 
> > `data：包含论文每一页`
> > 
> > `figures：存放图像，方便后期调整和修改`
> > 
> > `ref：集中管理参考文献`
> > 
> > 
> > <font color="gree"> 例如，如果想要修改摘要，就是修改`data\abstract.tex` </font>
> > 
> > > <div align=center>
> > > <img src="./images/overleaf_8.png"  style="zoom:100%"/>
> > > <img src="./images/overleaf_9.png"  style="zoom:100%"/>
> > > </div> 
> > 
> > 
> > <font color="gree"> 例如，如果想要添加图片，就是`Upload 到 figures 文件夹` </font>
> > 
> > > <div align=center>
> > > <img src="./images/overleaf_10.png"  style="zoom:100%"/>
> > > <img src="./images/overleaf_11.png"  style="zoom:100%"/>
> > > </div> 
> >  
> > 
> > <font color="gree"> 例如，如果想要修改参考文献，就是修改`ref\refs.bib`</font>
> > 
> > > <div align=center>
> > > <img src="./images/overleaf_12.png"  style="zoom:100%"/>
> > > </div> 
> >  
> > 
> 
> 
> <font color="pink">（4）论文封面如何修改 </font>
> 
> > `98%` 的内容，只需要通过修改 `data、figures、ref` 文件夹就行
> > 
> > `1%` 的内容，即论文标题等，对于清华大学模板，需要修改 `thusetup.tex`
> > 
> > > <div align=center>
> > > <img src="./images/overleaf_13.png"  style="zoom:100%"/>
> > > </div> 
> >  
>
> 
> 
> <font color="pink">（5）论文章节如何添加 </font>
>
> >  模板中只有4个章节 `ch01、ch02、ch03、ch04`，如何我们需要 `ch05` 呢？
> > 
> > `1%` 的内容，即论文结构、目录树等，对于清华大学模板，需要修改 `文档结构定义文件 thuthesis-example.tex`
> > 
> > > <div align=center>
> > > <img src="./images/overleaf_14.png"  style="zoom:100%"/>
> > > </div> 
> > 
> > * `data`中添加`data\chap05.tex`
> > 
> > * 打开`thuthesis-example.te`, 修改 `% 正文部分`, 实现增加章节的效果
> > 
> > > <div align=center>
> > > <img src="./images/overleaf_15.png"  style="zoom:100%"/>
> > > </div> 
> > 
> 
> 
> 
> 
> <font color="pink">（4）其他模板呢？ </font>
> 
> > 
> > <font color="yellow"> 
> > 
> > 即使是其他模板，我们也只需要关注 `.tex` 文件，这是需要我们自行编辑的文件
> > 
> > 想要快速找到文档结构定义文件，可以通过 `Menu` 中的 `Main document` 找到，默认的就是定义文档结构的文件
> > 
> > <div align=center>
> > <img src="./images/overleaf_16.png"  style="zoom:100%"/>
> > </div> 
> > 
> >  </font>
> > 
> > 
> 
> 
> 







#### LaTeX 从入门到够用（3）语法和常用命令（上）

> 
> 飞书云文档：https://xyfamily.feishu.cn/docx/MuhFdGc1lovo84xoq6pcScTSnbb
>
> Overleaf 帮助文档（强烈推荐）https://www.overleaf.com/learn
>
> LaTeX Cheatsheet 速查手册 `.\material\LaTeX Cheatsheet.pdf`
> 
> 第三期视频（上和下）中所涉及的 .tex 源文件 `.\material\六边形游乐场.tex`
> 
> 第三期视频（上和下）中所涉及的 PDF 文件 `.\material\六边形Up演示文档.pdf`
> 





> 
> <font color="gree"> 在清华大学模板的基础上，添加`data\chap05.tex`，内容从`六边形游乐场.tex`复制 </font>
> 
> > <div align=center>
> > <img src="./images/overleaf_17.png"  style="zoom:100%"/>
> > </div> 
> 
> 
> <font color="gree"> 修改 `文档结构定义文件 thuthesis-example.tex` </font>
> 
> > <div align=center>
> > <img src="./images/overleaf_18.png"  style="zoom:100%"/>
> > </div> 
> 
> 
> 
> 




> 
> 
> <font color="pink">（1） 注释  </font>
> 
> > 
> > `%` 开头的文字不会显示在右侧编译
> > 
> > ```latex
> > % 首先，什么是注释
> > % 右边的界面不会显示这里的内容
> > % 可以用来给自己写一些备注，或者隐藏掉废弃但是不舍得删除的内容
> > % 单行注释的语法：以百分号 % 开头
> > ```
> 
> <font color="pink">（2） 命令  </font>
> 
> > 编译器自动标出的蓝色部分，以反斜杠 `\`开头，以一个空格结束（还有其他方式）
> > 
> > <div align=center>
> > <img src="./images/overleaf_19.png"  style="zoom:100%"/>
> > </div> 
> > 
> > 命令和文字混排时，要记得：每次命令结束之后，给一个空格
> > 
> > ```latex
> > 命令是 LaTeX 里最基本的指令语句，以反斜杠开头，一般以空格结束，形态是：
> > 
> > \begin{verbatim}
> >     \command[可选参数]{必选参数}
> > \end{verbatim}
> > 
> > 关于命令的知识：
> > 0. 命令区分大小写； 
> > 1. 有些命令可以没有任何参数，比如说 \LaTeX；
> > 2. 如果一个命令有可选参数（不论有几个），都应该被写在[和]之间；
> > 3. 如果一个命令有必选参数（不论有几个），都应该被写在\{和\}之间。
> > ```
> > 
> > ```latex
> > 展示命令的两种方式（一般不用）
> > 1. 使用 verbatim 环境，上面已经用到了。
> > 2. 使用 \verb|| 命令，一般用在行内命令展示，例如 \verb|\item|
> > ```
> > 
> > <div align=center>
> > <img src="./images/overleaf_20.png"  style="zoom:100%"/>
> > </div> 
> > 
> 
> 
> <font color="pink">（3） 分段  </font>
> 
> > 代码中经常有空一行的情况，意思是重新分段
> >  
> > LaTeX 默认每段缩进
> > 
> > 当然对于有序列表来说，后续有更好的方式处理
> > 
> > <div align=center>
> > <img src="./images/overleaf_21.png"  style="zoom:100%"/>
> > </div> 
> > 
> > 
> 
> <font color="pink">（4）段内换行 </font>
> 
> > ```latex
> > 分段和换行是不一样的（可以从上面是否缩进看出来）
> > 1. 空一行 和 \par 命令是分一段
> > 2. \\ 和 \newline 命令是换一行
> > ```
> >  
> 
> 
> <font color="pink">（5）环境 </font>
> 
> > 
> > ```latex
> > 环境指被 \begin 和 \end 命令包围的空间，提供了相对独立的命令作用范围
> > 
> > 
> > 格式
> > \begin{环境名}
> >     ...
> > \end{环境名}
> > 
> > 环境演示：
> > \begin{verbatim}
> >     1. 这里就是 verbatim 环境里面
> >     2. 环境里的内容会收到这个环境的影响
> > \end{verbatim}
> > ```
> > 
> > <div align=center>
> > <img src="./images/overleaf_22.png"  style="zoom:100%"/>
> > </div> 
> > 
> 
> 
> 
> 
> <font color="pink">（6）包 </font>
> 
> > ```latex
> > LaTeX 本体包含了一些命令，
> > 
> > 但考虑到 LaTeX 被学术界广泛的使用， 需求多种多样，内置的命令很难满足所有的情况。
> > 
> > 因此，有了包的概念，每一个包都会提供很多新的命令。
> > 
> > 目前 LaTeX 生态有超过4000种的各种宏包，可以根据需要引入到你的文档里。
> > 
> > 一会我们下面插入图片的操作中，也会使用到特定的包。
> > ```
> > 
> 
> 
> <font color="pink">（7）代码结构 </font>
> 
> > 
> > 
> > 
> 
> 
> 
> 













