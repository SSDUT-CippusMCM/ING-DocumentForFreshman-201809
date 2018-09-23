# 数模组新人指南
## 公共讨论区，在文档还没有发布之前在这里讨论相关问题
&emsp;&emsp;编程语言是不是应该在常用软件里面单独地列出一类呢？ 感觉这个东西直接放到应用软件里面讨论，可能会有一些问题，可以在应用软件里面讨论软件的
IDE及可能需要的编译器会好一些

&emsp;&emsp;请大家如果觉得latex有什么好用的配置，或者其他系统（比如Mac）下latex的配置，都向“latex的安装”里加入qaq 因为只用过TeXLive+Winedt+SumatraPDF的配置，所以对其他配置的实用程度并不了解qaq。
## 编写这个文档可能需要注意的语法问题
```
#### XXX    
由于GitHub的一些特性 请在#后面加入空格，保证其标题的效果会显现    
&emsp;    
表示全角空格，可以在段首加入，以保证其缩进
如果需要贴图，可以看到仓库下面有Picture文件夹，上传到这里，然后利用markdown语法贴链接就行
如果是网络图片，那就直接贴链接（当然年头久了外链可能失效）
```
## 介绍及版权说明
&emsp;&emsp;数模组新生入门手册——长期维护> &lt;（使用GPL许可证  非商用授权 如果使用其中内容请表明出处）  
## 一、常用软件工具及基本配置方法（日常生活学习用）
### 1 系统软件
* 可以尝试安装archlinux系统来体验自定义安装操作系统的感觉。为什么是archlinux呢？原因如下:
	* 我们安装windows都是被引导着被动下一步，失去了自己给磁盘分区，设置引导，连接网络，安装自己喜欢的桌面环境等等很多过程。arch自由度比较高。
	* arhlinux滚动更新。
	* 可以使用pacman安装很多软件，只要mirrorlist里面有，pacman帮我们找到软件来源，用户只需要告诉他匹配的名字就好了。
* 挂载双系统：可以用grub挂载双系统．第二个系统和第一个系统共用EFI分区，这样就不用每次都进入Boot选择进入那个分区了。
 
### 2 应用软件

好的软件可以帮助我们提高办公学习效率以及编写代码的体验。

* **python**  
可以用Anaconda管理，IPython+JupiterNoteBook。
* **Typora**  
笔记软件，支持Markdown语法输入文字、Latex语法输入公式以及为不同语言提供高亮的代码块，可以利用CSS个性化主题，并且为Mac用户提供图床。缺点是字数较多时会卡顿。
* **Visual studio 2017**  
Visual Studio Community 2017 社区版为免费版本，在任务有网络的地方可以轻松下载获取。安装的过程中，几乎不需要任何的干预既可以安装完成，但安装VS要注意一定要安装社区版（Visual Studio Community 2017 社区版为免费版本，另外两个版本是收费的，安装了收费版本就卸载吧）；此外，下载最好在教学区等有不限流量网络的地方；其次，安装后出了问题不能打开、不能新建工程之类的，直接卸载（可用一开始下载的预安装程序卸载，卸载的干净），亲测好用。
[Visual studio 2017基本配置](https://blog.csdn.net/u010202588/article/details/79366328)

### 3 工具，脚本类  

* **Chrome插件HTML5 Video Speed Control**  
在Chrome看视频时可以调整倍速，对于在Chrome学习视频非常实用，比如b站“线性代数的本质”系列。

### 4 免费获取软件的重要工具——学校邮箱  
带有edu后缀的学校邮箱是非常有用的巨大福利！比如说良心好用还很贵的jetbrains全家桶，用学校邮箱都可以免费获取非常完整的版本，只需要通过简单的许可证认定；github、微软、谷歌、腾讯云、阿里云等也有教育策略。非常建议充分利用这个资源！
## 二、数学建模常用的两大软件Matlab与Latex的简单介绍及入门
### 1 Matlab

#### 1 Matlab的介绍

Matlab是matrix&laboratory两个词的组合，意为矩阵实验室。是由美国mathworks公司发布的主要面对科学计算、可视化以及交互式程序设计的高科技计算环境。Matlab可以进行矩阵运算、绘制函数和数据、实现算法、创建用户界面、连接其他编程语言的程序等，主要应用于工程计算、控制设计、信号处理与通讯、图像处理、信号检测、金融建模设计与分析等领域。  
在数模竞赛中，Matlab主要用于模型的求解，占有不可或缺的位置。另外，大一的工数与线代两门课也有Matlab上机，强烈建议尽早学习Matlab。
#### 2 Matlab的安装

可以自行下载安装包，学校也提供Matlab2018正版软件免费下载（但使用需要在dlut下）。具体安装步骤移步百度，都有十分详细的教程。安装时间比较长，建议在校园网环境下安装。  
[学校超算中心网址](http://hpc.dlut.edu.cn/)
* 大连理工大学超算中心的正版软件模块有MTALAB2018a的详细下载安装方法，建议把下面链接里的所有细节（MATLAB校园单机版安装指南、Windows版iso格式Matlab安装文件使用方法说明、Matlab许可证关联方法、Mathworks账户创建方法、大工云盘MATLAB校园单机版安装文件下载方法、Matlab功能说明）全看完再去安装。 Matlab-高性能计算中心链接如下（注意！要使用校园网才能打开链接）：
[ Matlab-高性能计算中心](http://hpc.dlut.edu.cn/jingyanjiaoliu/list.jsp?urltype=tree.TreeTempUrl&wbtreeid=1059)
#### 3 Matlab基础入门

* 安装完成之后，Matlab的界面有命令行窗口、工作区、文件路径等几个窗口。大家可以先尝试着在命令行窗口里面输入一些简单的运算，体验一下Matlab的一些简单操作。如果需要进行计算，可以直接在命令框中进行输入计算，回车就可以得出结果，同样，一些数学表达式也可以得出来。比如，输入“2+3”后点击回车，显示出了“ans = 5”的结果。输入“exp(3)”（求e的三次方）得到"ans = 20.0855"的结果。
```
>> 2+3

ans =

     5
>> exp(3)

ans =

   20.0855
```

* 如果不想直接在命令窗口输入，因为每次都得重新输入命令，比较麻烦。有一种简便的方法，建立m文件可以解决这个烦恼，点击”新建脚本”按钮，新建一个窗口，保存为.m格式的文件，在窗口输入指令，下次直接运行m文件即可出结果，修改只需在m文件修改即可，比较方便。

* 在命令行窗口中输入"clear"，敲击回车之后，就可以清空工作区中目前存在的变量。在命令行中输入"clc"，就可以清空历史窗口中的内容，但是其变量都不会消失。一般我们会选择输入“clear”、"回车"、"clc"、"回车"，然后重新对Matlab进行新的操作（这一系列操作的结果与关闭了软件之后再打开会得到一样的结果）。

* matlab的强大之处，不光在于它的矩阵计算与数值处理上，图形绘制也是它的一方面。例如，通过使用一些函数，可以绘制出"y=sinx"的曲线，还可以改变曲线的颜色、对图形进行标注等等。其中，plot是比较常用的一个功能比较强大的函数。

```
>> x=-pi:pi/20:pi;
plot(x,sin(x))
```

* 如果对Matlab的函数有任何疑问，可以通过help来查看**帮助文档**。  
在学习使用新的工具时，帮助文档非常有用！这也是为什么一定要学好英语。

#### 4 学习Matlab的书籍

学校图书馆关于Matlab的藏书非常丰富，**善用图书检索功能**。初学推荐借两本就够用了，一本作为工具书，随时查找，另一本与模型相关联，用它来学习解决问题。
* 卓金武.MATLAB在数学建模中的应用.北京航空航天大学出版社  
这本书的例题主要来自于国赛，有大量代码，对比赛很有帮助。同时还讲解了编程思想。
* 邓薇.MATLAB函数速查手册.人民邮电出版社  
非常有用方便的工具书。
### 2 Latex的介绍及安装

#### 1 Latex的介绍
> &emsp;&emsp;LaTeX， 是一种基于TEX的排版系统，由美国电脑学家莱斯利·兰伯特在20世纪80年代初期开发，利用这种格式，即使用户没有排版和程序设计的知识也可以充分发挥由TEX所提供的强大功能，能在几天，甚至几小时内生成很多具有书籍质量的印刷品。对于生成复杂表格和数学公式，这一点表现得尤为突出。因此它非常适用于生成高印刷质量的科技和数学类文档。这个系统同样适用于生成从简单的信件到完整书籍的所有其他种类的文档。

&emsp;&emsp;简单来说，Latex是用于生成PDF文档的编辑与排版软件，排版效果、对复杂公式的支持与对插图的支持相比Word更优秀。LaTeX编辑和排版的核心思想在于，通过\section和\paragraph等语句，规定了每一句话在文章中所从属的层次，从而极大方便了对各个层次批量处理。

#### 2 Latex的安装

##### TeX发行版的选择

|   OS   | TeX Distribution |
|   :--:   |   :--:   |
|  Windows  |  CTeX  |
|  Mac  |  MacTeX  |
|  Windows & Linux  |  TeXLive  |

&emsp;&emsp;Windows下推荐TeXLive，不推荐安装CTeX套装。关于TeXLive与MikTeX的对比，[点这里](https://tex.stackexchange.com/questions/20036/what-are-the-advantages-of-tex-live-over-miktex)。具体安装程序可以到搜索引擎搜索TeXLive，官网下载。

##### Latex编辑器的选择

&emsp;&emsp;Windows下最常用的编辑器是WinEdt，功能齐全，适合入门。收费应用，只有30天试用期，网上可以找到破解版。Sublime Text也可以，也是收费应用，轻量级，打开快，且代码高亮美观。

##### Latex中PDF阅读器的选择

&emsp;&emsp;较常用的是SumatraPDF，用于查看编译出来的PDF格式的论文。

##### WinEdt的环境配置

&emsp;&emsp;下载安装TeXLive与SumatraPDF后，需要在WinEdt中将其设置为默认的编译器与PDF阅读器。配置的具体步骤[点这里](https://blog.csdn.net/wr339988/article/details/66634637/)


### 3 Latex基础入门
#### 1 基本格式
* 文档的开始和结束
```
\documentclass[12pt]{ctexart}
\usepackage{graphicx}  %这里主要是插入一些宏包
\begin{document}
\section{1}
\subsection{123}
一些内容
\end{document}
```
* 一二三级标题
```
\section{}      %一级标题
\subsection{}   %二级标题
\subsubsection{}%三级标题
```
通常在中文论文写作中，一级标题用汉字书写，只需要添加一行
```
\CTEXsetup[number={\chinese{section}}]{section}
```
* 注释
	* 单行注释使用%
	* 多行注释
	```
	\usepackage{verbatim}
	\begin{comment}
	
	\end{comment}
	```
#### 2 插入图片
```
\usepackage{graphicx}
\begin{figure}[!h]
  \centering
   \includegraphics[width=0.8\textwidth]{picture.jpg}
  \caption{图片}
\end{figure}
```
需要注意的是，picture.jpg应与.tex处于同一目录下。同时，对于一些复杂格式的图片不能采用此方式保存。

#### 3 数学公式
* 公式语法
	* 下标使用_{下标内容}，上标使用^{上标内容}
	* 分式使用\dfrac{分子}{分母}
	* 希腊字母如β使用\beta
* 插入公式
	* 不换行公式
	```
	$x_{min}+x_{max}$
	\begin{math} 
	x_{min}+x_{max} 
	\end{math}
	```
	* 换行公式
	```
	\begin{equation} 
	x_{min}+x_{max} 
	\end{equation}
	```
若不希望对公式自动编号，则在equation后加一个*。

#### 4 三线表
```
\begin{table}[!h]
\centering
\begin{tabular}{ccccc} %c表示center居中，l表示left左对齐，r表示right右对齐
\toprule
Country& Life expectancy  &Population&Growth rate &Labour force  \\
\midrule
The U.S. & 77 &30.393& 1 &99  \\
Canada & 79 &3.077&1  &100 \\
China & 71 &133.42&0.8  &92 \\
Japan & 81 & 332.42&0.2  &100 \\
\bottomrule
\end{tabular}
\caption{Index data(Only a small part)}
\end{table}
```


#### 5 代码插入
```
\usepackage{listings}
\begin{lstlisting}[language=C++]
#include<iostream>
using namespace std;
int main()
{
    cout << "Hello, World!" << endl;
} 
\end{lstlisting}
```

## 三、OJ（Online Judge）的介绍及可能出现的问题
### 0 为什么要用OJ
多实践是熟练掌握一门语言的唯一途径，OJ是练习的很好平台
### 1 OJ的介绍
OJ是用来在线检测程序的判题系统，同时各大OJ平台上有大量的程序设计题目，刷题可以有效提高算法设计能力。题目往往都会给出**问题的描述、问题的输入和输出要求，并会给出几组样例数据**。OJ采用后台黑箱测试，测试数据非常全面，涵盖各种特殊情况，在结果的比对上也不放过一个空格和回车，对问题的输出格式要求非常严格。因此，在初次使用OJ时经常会出现各种各样的问题，导致无数次Wrong Answer的出现。
### 2 遇到Wrong Answer该怎么做？
* 检查输入输出格式  
对初学者来说，最可能的非代码逻辑错误Wrong Answer原因就是输入输出格式不正确，这个链接里面介绍了几种输入输出格式的写法：[点我](http://cscoder.iteye.com/blog/2306067)  
同时也要注意是否有多余空格输出、I64d or lld？输出浮点数的精度问题等等。(这样的失误也可能造成Presentation Error）
* 考虑边界数据和边界条件
* 检查数据类型是否正确
### 3 遇到其他系统返回信息该怎么做？
* 利用搜索引擎，查找返回信息所对应的常见问题，要学会自己debug
* 仔细认真地阅读题目和代码，思考自己的代码到底符不符合题意
* 不要放弃希望，成功ac一道题的整个过程中都是在一直进步的
## 四、电脑硬件知识的普及及选购建议

### １　笔记本选购心得

首先讲一讲买电脑要看哪些指标。

我们总是现有一些难以满足的需求：玩游戏，搞图形，多任务同时运行，等等。也可能卖笔记本是为了轻便易于携带。那么这些外在指标是如何从硬件指标里体现出来的呢？

关于处理器，现在比较流行i5,i7。它们的性能体现在开多个程序同时运行会不会卡。我们打开任务管理器的时候就可以看到各种任务占用的内存。越多内存占用大的程序可以并行，这个电脑越不容易卡。然而，这个容不容易卡不仅仅由处理器决定。实际上这也包含了访存过程，在CPU功能不断增强，I/O设备不断增多时，主存的存取速度已经成为计算机的瓶颈。当然，CPU并不是完全访问主存的阿，也有CPU访问Cache的情况，而在这种情况下Cache命中率便很重要。既然这个问题如此复杂，那我们选购该怎么判断呢？开好多个程序看卡不卡还是最简单的了。当然，i３及以下的还是不要考虑作为上学使用的了。

之后，说一下显卡选购。目前市场上比较流行３种显卡：英伟达（NVIDA）,AMD,Intel.有一种说法是AMD拥有极致色彩，NVIDA做到了曲线细分，Intel动态模糊......不管怎么说，如果想做图形学做渲染英伟达还是不错的。

### 2  整笔记本推荐

> "没钱就上船，船翻了就修或者买新的。一个外星人可以买两个船。"
							——神舟论坛言论

确实神舟笔记本可以以较少的钱换来更好的硬件体验，没有钱可以试一试。
有钱的话戴尔外星人比较耐用，五年前买的现在还能跑Steam上的主流游戏。但是外星人散热不是很好。雷蛇灵刃散热更优于外星人，但是价钱也更高。我自己不太玩大游戏，从小学起一直用ThinkPad,比较基本的体验就是键盘很舒服（内置机械键盘），以及可以脱离鼠标（小红点＋快捷键）。

Mac是工作上使用电脑的非常好的选择，还可以限制自己玩游戏，虽然有一点贵（--Hty）




## 五、如何问问题？
* 问问题之前
     * 试着通过 Google 等网络搜索引擎找到答案  (知之为知之，不知Google知)
     * 试着通过在技术社区，论坛搜索你的问题找到答案
     * 试着通过 debug （强烈建议尽早学习调试）或检查来找到答案
     * 试着通过问一个相关方面经验的朋友来找到答案
     * 试着通过阅读源代码来找到答案
* 当你问问题时
     * 组织问题：首先要把问题组织一下，让我们看懂你问的问题；尽量避免  先喊人 再问问题
     * 整理问题：把自己遇到的问题，在上述五种基础上认真寻找答案，如果没找到答案，就把相关的问题链接和你搜索到的答案整理一下,这样准备充分，便于在和别人探讨时深入交流
     * 精确描述：明确地说出你的问题或观点，尽可能描述你提出这个问题发生的背景，说明你在提问前是怎样去研究和理解这个问题的，说明你在提问前采取了什么步骤去解决
* 得到解答后
     * 思考并整理思路
     * 最好写一个文档来记录自己遇到的问题们
     * 建议维护自己的技术博客


## 六、优秀课外书籍推荐

* PPT制作相关——标题含图表术的都可以看看
* Latex论文写作入门——正确写作美国大学生数学竞赛论文
* 高等数学——前期可以做吉米多维奇 中后期考研真题（吉米多维奇可能不是很建议---hty）
* 线性代数——线性代数应该这样学（比较难懂，但是思路和我们的教材不一样 答案在网上可以找到
* 英语学习——为了英文参考文献的阅读和英语论文的书写，我们需要有好的英语水平。由于数模比赛内容宽泛，可以在学英语的同时了解跨学科知识，比如政治经济新闻。推荐the Econmoist，Monocle,etc.


## 七、常见其它问题FAQ
* Mac端常用软件推荐	
	* C或C++的编译器CLion。CLion是一款专为开发C及C++所设计的跨平台IDE，Windows、Linux、Mac下都支持CLion。虽然CLion收费，但是可以在官网上凭借学生优惠安装，用校园邮箱验证信息
	* 只用于Mac下的集成开发编译器Xcode。Xcode是Mac上相似于VS在Windows中的一款编辑器，负责Apple平台的所有应用开发，Xcode中可以选择不同语言自如使用，如C、C++、Swift、Objective-C等
	* Eclipse。Eclipse主要用于Java或JavaWeb程序的开发
	* Pycharm。一款有免费版的用于Python语言的IDE
	* CAJViewerMac。一款用于查看.caj文件(从知网下载的论文格式)的软件
	* The Unarchiver。Mac下的解压软件
	* 迅雷、百度云。老司机都懂
	* virtualbox。较为好用的虚拟机管理工具
	* mysql或postgresql，数据库。Mac下没有sqlserver
	* Appache Tomcat服务器
	* Vim是极为好用的编辑工具，尽管有一定的学习成本
	* Sublime编辑 + 终端下编译 也是极为好用的工具 
	* 其他。有很多好用的软件同时也具有Mac端的版本，如Office、Matlab、CS系列等，虽然资源比较难找，但耐心百度总是有的
* Mac下Python包管理工具:pip3、homebrew
* Mac下配置环境：和Windows直接修改不同，Mac端通常需要更改bash_profile配置文件
## 八、友情链接
* 欢迎大家我的关注我的知乎专栏，地址为https://zhuanlan.zhihu.com/duduru 内容是关于深度学习，机器学习。可能现在接触对大家有点早，不过还是推荐一下

