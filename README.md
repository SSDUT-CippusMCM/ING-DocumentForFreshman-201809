# 数模组新人指南

## 介绍及版权说明

数模组新生入门手册 —— 长期维护 > <（使用 GPL 许可证  非商用授权 如果使用其中内容请表明出处）  

## 常用软件工具及基本配置方法（日常生活学习用）

### 系统软件

* 可以尝试安装 [Arch Linux 系统](https://www.archlinux.org/)来体验自定义安装操作系统的感觉。为什么是 Arch Linux 呢？原因如下:
	* 我们安装 Windows 都是被引导着被动下一步，失去了自己给磁盘分区，设置引导，连接网络，安装自己喜欢的桌面环境等等很多过程。Arch 自由度比较高。
	* Arch Linux 滚动更新。
	* Arch Linux [官方 Wiki](https://wiki.archlinux.org/) 非常全面，涵盖面很广。
	* 可以使用 [`pacman`](https://wiki.archlinux.org/index.php/Pacman) 安装很多软件，只要 `mirrorlist` 里面有，`pacman` 帮我们找到软件来源，用户只需要告诉他匹配的名字就好了。
	* 还可以直接使用 [`yay`](https://github.com/yaybu/yay) 来安装，并且配上[清华源](https://mirrors.tuna.tsinghua.edu.cn/)。
* 挂载双系统：可以用 `grub` 挂载双系统．第二个系统和第一个系统共用 EFI 分区，这样就不用每次都进入 Boot 选择进入那个分区了。
 
### 应用软件

好的软件可以帮助我们提高办公学习效率以及编写代码的体验。

* [**Python**](https://www.python.org/)  
	可以用 [Anaconda](https://www.anaconda.com) 管理，IPython + [Jupyter](https://jupyter.org)。如果觉得 Anaconda 太大，还可以使用 [Miniconda](https://docs.conda.io/en/latest/miniconda.html) 然后使用 [conda-forge](https://conda-forge.org/) 社区维护的版本，自定义需要的软件。（依然有清华源）
* [**Typora**](https://typora.io)  
	笔记软件，支持 Markdown 语法输入文字、LaTeX 语法输入数学公式以及为不同语言提供高亮的代码块，可以利用 CSS 个性化主题，并且为 Mac 用户提供图床。缺点是字数较多时会卡顿（因为使用了 Electron 框架）。
* [**Visual Studio 2019**](https://visualstudio.microsoft.com/)  
	Visual Studio Community 2019 社区版为免费版本，在任务有网络的地方可以轻松下载获取。安装的过程中，几乎不需要任何的干预既可以安装完成，但安装 VS 要注意一定要安装社区版（Visual Studio Community 2019 社区版为免费版本，另外两个版本是收费的，安装了收费版本就卸载吧）；此外，下载最好在教学区等有不限流量网络的地方；其次，安装后出了问题不能打开、不能新建工程之类的，直接卸载（可用一开始下载的预安装程序卸载，卸载的干净），亲测好用。
	[Visual Studio 2017 基本配置](https://blog.csdn.net/u010202588/article/details/79366328)
* [**Code::Blocks**](http://www.codeblocks.org/)  
	Code::Blocks 是初学者常用的 C/C++ IDE。它也是很好的跨平台 IDE，界面干净利落，支持语法彩色醒目显示，支持代码完成，支持工程管理、项目构建、调试。Code::Blocks 对初学者十分友好，其代码补全功能可以大大提升写代码速度。
* [**Dev-C++**](https://sourceforge.net/projects/dev-cpp/)  
	Dev-C++ 是一款适合初学者的轻量级 C/C++ 集成开发环境（IDE），开发环境包括多页面窗口、工程编辑器以及调试器等，在工程编辑器中集合了编辑器、编译器、连接程序和执行程序，提供高亮度语法显示的，以减少编辑错误，还有完善的调试功能，适合初学者与编程高手的不同需求。
* [**Sublime Text**](https://www.sublimetext.com/)  
	Sublime Text 是一个代码编辑器，Sublime Text 具有漂亮的用户界面和强大的功能，例如代码缩略图，Python 的插件，代码段等。还可自定义键绑定，菜单和工具栏。Sublime Text 的主要功能包括：拼写检查、书签、完整的 Python API、Goto 功能、即时项目切换、多选择、多窗口等等。Sublime Text 是一个跨平台的编辑器，同时支持 Windows、Linux、Mac OS X 等操作系统。支持多重插件，大大扩展其功能。
* [**Visual Studio Code**](https://code.visualstudio.com)  
	这不是 Visual Studio，Visual Studio Code 是一个代码编辑器，用户界面漂亮，[丰富的插件](https://code.visualstudio.com/docs/editor/extension-gallery)，跨平台支持（同时支持 Windows、Linux、Mac OS X 等操作系统），内置 Git 支持，最重要的是它不像 Sublime Text 要收费，它是开源免费软件。

### 工具，脚本类

* **Chrome 插件 HTML5 Video Speed Control**  
	在 Chrome 看视频时可以调整倍速，对于在 Chrome 学习视频非常实用，比如 B 站 [3Blue1Brown](https://www.3blue1brown.com/) 出品的[《线性代数的本质》系列](https://www.bilibili.com/video/av6731067)（强烈推荐看看，尤其是当你看了让人蒙圈的国内线代教材）。
* [**Tampermonkey**](https://www.tampermonkey.net/) 油猴脚本

### 免费获取软件的重要工具 —— 学校邮箱  

带有 edu 后缀的学校邮箱是非常有用的巨大福利！比如说良心好用还很贵的 [JetBrains](https://www.jetbrains.com/) 全家桶，用学校邮箱都可以免费获取非常完整的版本，只需要通过简单的许可证认定；GitHub 可以领[学生背包](https://education.github.com/pack)，里面有很多很好的东西；微软、谷歌、腾讯云、阿里云等也有教育策略。非常建议充分利用这个资源！

## 数学建模常用的两大软件 MATLAB 与 LaTeX 的简单介绍及入门

### MATLAB

#### MATLAB 的介绍

[MATLAB](https://www.mathworks.com/products/matlab.html) 是 matrix & laboratory 两个词的组合，意为矩阵实验室。是由美国 MathWorks 公司发布的主要面对科学计算、可视化以及交互式程序设计的高科技计算环境。MATLAB 可以进行矩阵运算、绘制函数和数据、实现算法、创建用户界面、连接其他编程语言的程序等，主要应用于工程计算、控制设计、信号处理与通讯、图像处理、信号检测、金融建模设计与分析等领域。

在数模竞赛中，MATLAB 主要用于模型的求解，占有不可或缺的位置。另外，大一的工数与线代两门课也有 MATLAB 上机，强烈建议尽早学习 MATLAB。

#### MATLAB 的安装

可以自行下载安装包，学校也提供 MATLAB 2018 正版软件免费下载（但使用需要在 DLUT 下）。具体安装步骤移步百度，都有十分详细的教程。安装时间比较长，建议在校园网环境下安装。([学校超算中心网址](https://hpc.dlut.edu.cn/))

* 大连理工大学超算中心的正版软件模块有 MATLAB 2018a 的详细下载安装方法，建议把下面链接里的所有细节（MATLAB 校园单机版安装指南、Windows 版 `iso` 格式 MATLAB 安装文件使用方法说明、MATLAB 许可证关联方法、MathWorks 账户创建方法、大工云盘 MATLAB 校园单机版安装文件下载方法、MATLAB 功能说明）全看完再去安装。 MATLAB - 高性能计算中心链接如下：[MATLAB-超算中心网站](https://hpc.dlut.edu.cn/cszy/syrj/MATLAB.htm)

#### MATLAB 基础入门

* 安装完成之后，MATLAB 的界面有命令行窗口、工作区、文件路径等几个窗口。大家可以先尝试着在命令行窗口里面输入一些简单的运算，体验一下 MATLAB 的一些简单操作。如果需要进行计算，可以直接在命令框中进行输入计算，回车就可以得出结果，同样，一些数学表达式也可以得出来。比如，输入 `2+3` 后回车，显示出了 `ans = 5` 的结果。输入 `exp (3)`（求 ![e^3](https://latex.codecogs.com/svg.latex?e%5E3)）得到 `ans = 20.0855` 的结果。

	```matlab
	>> 2+3

	ans =

	     5
	>> exp (3)

	ans =

	   20.0855
	```

* 如果不想直接在命令窗口输入，因为每次都得重新输入命令，比较麻烦。有一种简便的方法，建立 `m` 文件可以解决这个烦恼，点击“新建脚本”按钮，新建一个窗口，保存为 `.m` 格式的文件，在窗口输入指令，下次直接运行 `m` 文件即可出结果，修改只需在 `m` 文件修改即可，比较方便。

* 在命令行窗口中输入 `clear`，敲击回车之后，就可以清空工作区中目前存在的变量。在命令行中输入 `clc`，就可以清空历史窗口中的内容，但是其变量都不会消失。一般我们会选择输入 `clear`、<kbd>回车</kbd>、`clc`、<kbd>回车</kbd>，然后重新对 MATLAB 进行新的操作（这一系列操作的结果与关闭了软件之后再打开会得到一样的结果）。

* MATLAB 的强大之处，不光在于它的矩阵计算与数值处理上，图形绘制也是它的一方面。例如，通过使用一些函数，可以绘制出 ![y=\sin x](https://latex.codecogs.com/svg.latex?y%3D%5Csin%20x) 的曲线，还可以改变曲线的颜色、对图形进行标注等等。其中，`plot` 是比较常用的一个功能比较强大的函数。

	```matlab
	>> x=-pi:pi/20:pi;
	plot (x,sin (x))
	```

* 如果对 MATLAB 的函数有任何疑问，可以通过 `help` 来查看**帮助文档**。

	在学习使用新的工具时，帮助文档非常有用！这也是为什么一定要学好英语。

#### 学习 MATLAB 的书籍

学校图书馆关于 MATLAB 的藏书非常丰富，**善用图书检索功能**。初学推荐借两本就够用了，一本作为工具书，随时查找，另一本与模型相关联，用它来学习解决问题。

* 卓金武，MATLAB 在数学建模中的应用，北京航空航天大学出版社  
	这本书的例题主要来自于国赛，有大量代码，对比赛很有帮助。同时还讲解了编程思想。
* 邓薇，MATLAB 函数速查手册，人民邮电出版社  
	非常有用方便的工具书。

### LaTeX 的介绍、安装与入门

#### LaTeX 的介绍

> LaTeX，是一种基于 TeX 的排版系统，由美国电脑学家莱斯利·兰伯特在 20 世纪 80 年代初期开发，利用这种格式，即使用户没有排版和程序设计的知识也可以充分发挥由 TeX 所提供的强大功能，能在几天，甚至几小时内生成很多具有书籍质量的印刷品。对于生成复杂表格和数学公式，这一点表现得尤为突出。因此它非常适用于生成高印刷质量的科技和数学类文档。这个系统同样适用于生成从简单的信件到完整书籍的所有其他种类的文档。

简单来说，LaTeX 是用于生成 PDF 文档的编辑与排版软件，排版效果、对复杂公式的支持与对插图的支持相比 Word 更优秀。LaTeX 编辑和排版的核心思想在于，通过 `\section` 和 `\paragraph` 等语句，规定了每一句话在文章中所从属的层次，从而极大方便了对各个层次批量处理。

#### LaTeX 的安装

- [TeX Live 下载及安装说明](https://liam.page/texlive/)

#### LaTeX 的入门

先看这份

- [一份其实很短的 LaTeX 入门文档](https://liam.page/2014/09/08/latex-introduction/)

如果这份内容不够，再看这份

- [一份不太简短的 LaTeX 2ε 介绍 （PDF版）](http://mirrors.ctan.org/info/lshort/chinese/lshort-zh-cn.pdf)

如果还有一些地方找不到，请用英文进行 Google 搜索，你会解决 99% 的问题（只要你不碰黑暗的底层原理）。

## OJ（Online Judge）的介绍及可能出现的问题

### 为什么要用 OJ

多实践是熟练掌握一门语言的唯一途径，OJ 是练习的很好平台

### OJ 的介绍

OJ 是用来在线检测程序的判题系统，同时各大 OJ 平台上有大量的程序设计题目，刷题可以有效提高算法设计能力。题目往往都会给出**问题的描述、问题的输入和输出要求，并会给出几组样例数据**。OJ 采用后台黑箱测试，测试数据非常全面，涵盖各种特殊情况，在结果的比对上也不放过一个空格和回车，对问题的输出格式要求非常严格。因此，在初次使用 OJ 时经常会出现各种各样的问题，导致无数次 Wrong Answer 的出现。

### 遇到 Wrong Answer 该怎么做？

* 检查输入输出格式

  对初学者来说，最可能的非代码逻辑错误 Wrong Answer 原因就是输入输出格式不正确，这个链接里面介绍了几种输入输出格式的写法：[点我](https://cscoder.iteye.com/blog/2306067)

  同时也要注意是否有多余空格输出、I64d or lld？输出浮点数的精度问题等等。（这样的失误也可能造成 Presentation Error）

* 考虑边界数据和边界条件
* 检查数据类型是否正确

### 遇到其他系统返回信息该怎么做？

* 利用搜索引擎，查找返回信息所对应的常见问题，要学会自己 debug
* 仔细认真地阅读题目和代码，思考自己的代码到底符不符合题意
* 不要放弃希望，成功 AC 一道题的整个过程中都是在一直进步的

## 电脑硬件知识的普及及选购建议

> 请注意，本部分只作为硬件知识选购的一个科普，非专业推荐，无利益相关。由于大部分的学长学姐一年以上没有买电脑了，所以消息可能有迟滞性如有同学想增添相关知识，请私发给副组，我们会增添上内容并注明作者。

### 笔记本选购心得

首先讲一讲买电脑要看哪些指标。

我们总是现有一些难以满足的需求：玩游戏，搞图形，多任务同时运行，等等。也可能卖笔记本是为了轻便易于携带。那么这些外在指标是如何从硬件指标里体现出来的呢？

关于处理器，现在比较流行 i5、i7 <sup><a id="footnote-cpu_gen-ref" href="#footnote-cpu_gen">[1]</a></sup>，它们的性能体现在开多个程序同时运行会不会卡。我们打开任务管理器的时候就可以看到各种任务占用的内存。越多内存占用大的程序可以并行，这个电脑越不容易卡。然而，这个容不容易卡不仅仅由处理器决定。实际上这也包含了访存过程，在 CPU 功能不断增强，I/O 设备不断增多时，主存的存取速度已经成为计算机的瓶颈。当然，CPU 并不是完全访问主存的阿，也有 CPU 访问 Cache 的情况，而在这种情况下 Cache 命中率便很重要。既然这个问题如此复杂，那我们选购该怎么判断呢？开好多个程序看卡不卡还是最简单的了。当然，i3 及以下的还是不要考虑作为上学使用的了。

关于市面上笔记本常见的 CPU 型号，我们经常能够看到在处理器型号后面带一个字母 U 或 H，例如 “第八代智能英特尔 ® 酷睿™ i7-8750H 处理器”，“第八代智能英特尔 ® 酷睿™ i7-8550U 处理器”。U 表示 Ultra Low Voltage，即超低电压版 CPU，这种型号的 CPU 功耗较低，延长了续航时间，但是性能能会受到一定的影响，例如超极本上常使用这种 CPU。H 代表高电压，这种 CPU 性能较优，但是续航能力较低。<sup><a id="footnote-cpu_lie-ref" href="#footnote-cpu_lie">[2]</a></sup>

如果想了解更多关于 CPU 型号及其代表，可以参考这篇文章 https://www.cnblogs.com/ArsenalfanInECNU/p/6903771.html?utm_source=debugrun&utm_medium=referral

之后，说一下显卡选购。目前市场上比较流行 3 种显卡：英伟达（NVIDA）、AMD、Intel。有一种说法是 AMD 拥有极致色彩，NVIDA 做到了曲线细分，Intel 动态模糊……不管怎么说，如果想做图形学做渲染英伟达还是不错的。<sup><a id="footnote-gpu-ref" href="#footnote-gpu">[3]</a></sup>

硬盘有两种：机械硬盘和固态硬盘 (SSD)。机械硬盘速度很慢，但容量可以很大，价格较便宜，适合用作数据盘。固态硬盘速度很快，大容量的 SSD 更是昂贵，个人建议购买 0.5 TB 或 256 GB 固态硬盘，用作系统盘<sup><a id="footnote-ssd-ref" href="#footnote-ssd">[4]</a></sup>。

---

<p id="footnote-cpu_gen"> <sup>[1]</sup> 此处泛指多核处理器，不谈代数谈 i5、i7 都是耍流氓，所以本段默认理解为 8 代就好了，当然你可以选择使用志强 Xeon 系列处理器。<a href="#footnote-cpu_gen-ref">&#8617;</a></p>

<p id="footnote-cpu_lie"> <sup>[2]</sup> 某些无良商家用带 U 的 i7 谎称比标准电压的 i5 好，当然现在可能不多见了。<a href="#footnote-cpu_lie-ref">&#8617;</a></p>

<p id="footnote-gpu"> <sup>[3]</sup> 大部分的机器学习相关框架只支持 N 卡 (英伟达显卡), 还有诸如 940MX、MX150、MX110 之类的都是较弱的 Nvidia 显卡，大型游戏之类的跑得动，所谓性价比较高的显卡应该是 GTX1060。另，本段所提到的 Intel 显卡都是集成显卡，并非独立显卡。一般情况下会随 Intel CPU 附带。<a href="#footnote-gpu-ref">&#8617;</a></p>

<p id="footnote-ssd">  <sup>[4]</sup> 用了之后就不想换回来。<a href="#footnote-ssd-ref">&#8617;</a></p>


### 整笔记本推荐

> “没钱就上船，船翻了就修或者买新的。一个外星人可以买两个船。”
> 
> —— 神舟论坛言论

确实神舟笔记本可以以较少的钱换来更好的硬件体验，没有钱可以试一试。

有钱的话戴尔外星人比较耐用，五年前买的现在还能跑 Steam 上的主流游戏。但是外星人散热不是很好。雷蛇灵刃散热更优于外星人，但是价钱也更高。我自己不太玩大游戏，从小学起一直用 ThinkPad, 比较基本的体验就是键盘很舒服，以及可以脱离鼠标（小红点＋快捷键）。（笔记本用机械键盘的很少，一般都是薄膜键盘）

惠普电脑没有多余的系统保护，相对联想和戴尔，惠普对用户开放的权限更大，作为开发人员，这种开放权限较大的笔记本是值得入手的。推荐惠普 ENVY 系列，轻薄，可以触屏，方便记笔记，适合学习。有钱的话，微软的 Surface pro 也可考虑，Surface pro 是平板笔记本两用的，可分离式键盘，可以单独选购触控笔，价格随配置变化

Mac 是工作上使用电脑的非常好的选择，还可以限制自己玩游戏，虽然有一点贵（——Hty）

Dell 电脑一般性价较低，可分为一下系列：

* Inspiron 灵越：适用于家庭和家庭办公经济实惠的笔记本电脑和二合一 PC，可提供多用途的日常计算功能；
* XPS：配备优质高分辨率显示屏，可呈现超凡的色彩、声音和流媒体效果；
* Alienware 外星人：高性能游戏体验，配备卓越的显卡和智能 Intel® Core™ 处理器，性能强劲；
* 等等……

Dell 笔记本电脑售后服务较为贴心，购买后一年内可免费上门维修，免费维修和更换软件和硬件<sup><a id="footnote-dell_service" href="#footnote-dell_service-ref">[1]</a></sup>。

---

<p id="footnote-dell_service"> <sup>[1]</sup> 某些机型非人为故障三次以上可以更换整机，以上所说的保修情况不同机型是不同的，选购之前需注意<a href="#footnote-dell_service-ref">&#8617;</a></p>


## 如何问问题？

* 问问题之前
     * 试着通过 Google 等网络搜索引擎找到答案  (知之为知之，不知 Google 知)
     * 试着通过在技术社区，论坛搜索你的问题找到答案
     * 试着通过 debug（强烈建议尽早学习调试）或检查来找到答案
     * 试着通过问一个相关方面经验的朋友来找到答案
     * 试着通过阅读源代码来找到答案
* 当你问问题时
     * 组织问题：首先要把问题组织一下，让我们看懂你问的问题；尽量避免  先喊人 再问问题
     * 整理问题：把自己遇到的问题，在上述五种基础上认真寻找答案，如果没找到答案，就把相关的问题链接和你搜索到的答案整理一下，这样准备充分，便于在和别人探讨时深入交流
     * 精确描述：明确地说出你的问题或观点，尽可能描述你提出这个问题发生的背景，说明你在提问前是怎样去研究和理解这个问题的，说明你在提问前采取了什么步骤去解决
* 得到解答后
     * 思考并整理思路
     * 最好写一个文档来记录自己遇到的问题们
     * 建议维护自己的技术博客


## 优秀课外书籍推荐

* PPT 制作相关 —— 标题含图表术的都可以看看
* LaTeX 论文写作入门 —— 正确写作美国大学生数学竞赛论文
* 高等数学 —— 前期可以做吉米多维奇 中后期考研真题（吉米多维奇可能不是很建议 ——hty）
* 线性代数 —— David C. Lay《线性代数及其应用》（比国内大多数教材都要好懂，重点在本质而不是计算，可以配合前面提到的《线性代数的本质》一起食用）、Sheldon Axler《线性代数应该这样学》（比较难懂，国外本科数学系教材，答案在网上可以找到）
* 英语学习 —— 为了英文参考文献的阅读和英语论文的书写，我们需要有好的英语水平。由于数模比赛内容宽泛，可以在学英语的同时了解跨学科知识，比如政治经济新闻。推荐 *the Econmoist*，*Monocle*, etc.
* [廖雪峰的官方网站，有不少优质的资源](https://liaoxuefeng.com/)

## 常见其它问题 FAQ

* Mac 端常用软件推荐	
	* C 或 C++ 的编译器 CLion。CLion 是一款专为开发 C 及 C++ 所设计的跨平台 IDE，Windows、Linux、Mac 下都支持 CLion。虽然 CLion 收费，但是可以在官网上凭借学生优惠安装，用校园邮箱验证信息
	* 只用于 Mac 下的集成开发编译器 Xcode。Xcode 是 Mac 上相似于 VS 在 Windows 中的一款编辑器，负责 Apple 平台的所有应用开发，Xcode 中可以选择不同语言自如使用，如 C、C++、Swift、Objective-C 等
	* [Eclipse](https://www.eclipse.org)。Eclipse 主要用于 Java 或 JavaWeb 程序的开发
	* [Pycharm](https://www.jetbrains.com/pycharm/)。一款有免费版的用于 Python 语言的 IDE
	* CAJViewerMac。一款用于查看 `.caj` 文件 (从知网下载的论文格式) 的软件
	* The Unarchiver。Mac 下的解压软件
	* 迅雷、百度云。老司机都懂
	* [VirtualBox](https://www.virtualbox.org)。较为好用的虚拟机管理工具
	* [MySQL](https://www.mysql.com/) 或 PostgreSQL，数据库。Mac 下没有 SQL Server
	* [Appache Tomcat](https://tomcat.apache.org/) 服务器
	* [Vim](https://www.vim.org/) 是极为好用的编辑工具，尽管有一定的学习成本
	* [Sublime](https://www.sublimetext.com/) 编辑 + 终端下编译 也是极为好用的工具 
	* 其他。有很多好用的软件同时也具有 Mac 端的版本，如 Office、MATLAB、CS 系列等，虽然资源比较难找，但耐心百度总是有的
* Mac 下 Python 包管理工具：Anaconda（简单介绍见前文）
* Mac 下软件包管理工具：[HomeBrew](https://brew.sh/)
* Mac 下配置环境：和 Windows 直接修改不同，Mac 端通常需要更改 `.bash_profile` 等配置文件

## 友情链接

* 欢迎大家我的关注我的知乎专栏，地址为 https://zhuanlan.zhihu.com/duduru 内容是关于深度学习，机器学习。可能现在接触对大家有点早，不过还是推荐一下
	
	—— 胡天翼，数模群联系我，群名片为 “皮皮抒琦”
