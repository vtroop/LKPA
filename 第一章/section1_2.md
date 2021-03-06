## **1.2 开放源代码的Unix/Linux操作系统**

&emsp;&emsp;在操作系统的历史上，Unix的生存周期最长。从Unix年诞生以来，虽然已经使用了40多年，但仍然是现有操作系统中最强大和优秀的系统之一。
 
### **1.2.1 Unix诞生和发展**

&emsp;&emsp;1965年在美国国防部高级研究计划署ARPA的支持下，麻省理工学院、贝尔实验室和通用电气公司决定开发一种“公用计算服务系统”， 希望能够同时支持整个波士顿所有的分时用户。该系统称作**MULTICS (MULTiplexed Information and Computing Service )。**

&emsp;&emsp;MULTICS设计目标是通过电话线把远程终端接入计算机主机。但是，MULTICS研制难度超出了所有人预料。长期研制工作达不到预期目标，1969年4月贝尔实验室退出，通用电气公司也退出了。 但最终，经过多年的努力，MULTICS 成功地应用了。运行MULTICS的计算机系统在九十年代中陆续被关闭。

&emsp;&emsp;MULTICS引入了许多现代操作系统领域的概念雏形，对随后操作系统特别是Unix的成功有着巨大的影响。

&emsp;&emsp;1969年,贝尔退出MULTICS研制项目后, Ken Thompson和Dennis M. Ritchie两个研究人员想申请经费购买计算机从事操作系统研究，但多次申请得不到批准。项目无着落，他们边在一台无人用的PDP-7上重新摆弄原先在 MULTICS 项目上设计的“空间旅行”游戏。为了使游戏能够在PDP-7上顺利运行,他们陆续开发了浮点运算软件包、显示驱动软件，设计了文件系统、实用程序、shell 和汇编程序。 1970年, 在一切完成后, 给新系统起了个同 MULTICS发音相近的名字Unix。随后, Unix用C语言全部重写, 自此, Unix诞生了。

&emsp;&emsp;Unix是现代操作系统的代表。Unix运行时的安全性、可靠性以及强大的计算能力赢得广大用户的信赖。促使Unix系统成功的因素有三点， 首先, 由于Unix是用C语言编写, 因此它是可移植的，它可以运行在笔记本计算机、PC机、工作站直至巨型机上；第二, 系统源代码非常有效, 系统容易适应特殊的需求。最后, 也是最重要的一点, 它是一个良好的、通用的、多用户、多任务、分时操作系统。

&emsp;&emsp;尽管Unix已经不再是一个实验室项目了，但它仍然伴随着操作系统设计技术的进步而继续成长，人们仍然可以把它作为一个通用的操作系统用于研究和演练。不过，因为Unix最终变为一个商业操作系统，只有那些能负担得起许可费的企业才用得起，这限制了它的应用范围。Linux的出现完全改变了这种局面。

### **1.2.2 Linux诞生**

&emsp;&emsp;Linux的第一个版本诞生于1991年，它的作者就是Linus Torvalds，这个芬兰小伙最初在做一个调度系统的作业时，福至心灵，他突发灵感开始着手将其改造为一个实用的操作系统。在开发初期，他借助了最负盛名的教育类操作系统Minix的一些思想和成果，但他有自己的雄心，要把自己这个系统变得比Minix更实用、更强健。他决定把自己的系统代码公布于众，并且欢迎任何人来帮助修改和扩充Linux系统，Linux选择了备受推崇的Unix系统接口标准（POSIX标准），由此Linux成为Unix风格操作系统家族中的一员，而且是一个代码完全公开的操作系统。

&emsp;&emsp;Linux的生命力来自于它的开源思想，自Linus公开Linux代码以来，世界各地的软件工程师和爱好者不断积极地对Linux系统进行修改和加强，将其版本从0.1 提高到2.0 、2.2、2.4、2.6，一直到如今的3.0，同时Linux也被从初期的x86平台移植到了PowerPC、Arm，Sparc、MIPS、68K等几乎市面上能找到的所有体系结构上，尤其是建立在Linux之上的Android系统，大大加强了Linux系统的实用性。

&emsp;&emsp;Linux作为开源软件皇冠上的明珠，越来越受到欢迎，毫无疑问地成为人气最旺，最活跃的GNU项目，围绕Linux社区内各种组织雨后春笋般地出现，Linux必将在教育领域、在工业领域取得更大的成功。

### **1.2.3操作系统标准POSIX**

&emsp;&emsp;POSIX 表示可移植操作系统接口（Portable Operating System Interface）。该标准由IEEE制订，并由国际标准化组织接受为国际标准。POSIX是在Unix标准化过程中出现的产物。到目前为止，POSIX已成为一个涵盖范围很广的标准体系，己经颁布了20多个相关标准，其中POSIX 1003.1标准定义了一个最小的Unix操作系统接口。也就是说，1003.1标准给出了一组函数的定义，至于如何实现，标准并不关注；或者说POSIX 1003.1提供了一种机制，而具体的策略由实现者决定。

&emsp;&emsp;任何操作系统只有符合POSIX 1003.1这一标准，就可以运行Unix程序。Linux在设计时遵循这一标准，因此，凡是在Unix上运行的应用程序几乎都可以在Linux上运行，这也是Linux得以流行的原因之一。

### **1.2.4 GNU 和 Linux**

&emsp;&emsp;GNU 是 GNU Is Not Unix 的递归缩写，是自由软件基金会的一个项目，该项目的目标是开发一个自由的 Unix 版本，这一 Unix 版本称为 HURD。尽管 HURD 尚未完成，但 GNU 项目已经开发了许多高质量的编程工具，包括 emacs 编辑器、著名的 GNU C 和 C++ 编译器（gcc 和 g++），这些编译器可以在任何计算机系统上运行。所有的 GNU 软件和派生工作均适用 GNU 通用公共许可证，即 GPL。GPL 允许软件作者拥有软件版权，但授予其他任何人以合法复制、发行和修改软件的权利。

&emsp; &emsp;Linux 的开发使用了许多 GNU 工具。Linux 系统上用于实现 POSIX.2 标准的工具几乎都是 GNU 项目开发的，Linux 内核、GNU 工具以及其他一些自由软件组成了人们常说的 Linux系统或Linux发布版：
 
1.	符合 POSIX 标准的操作系统内核、 Shell 和外围工具。 
2.	C 语言编译器和其他开发工具及函数库。
3.	X Window 窗口系统。 
4.	各种应用软件，包括字处理软件、图象处理软件等。 
5.	其他各种 Internet 软件，包括 FTP 服务器、WWW 服务器等。 
6.	关系数据库管理系统等。
 
### **1.2.5 Linux的开发模式**

&emsp;&emsp;Linux是一大批广泛分布于世界各地的软件爱好者，以互联网为纽带，通过BBS、新闻组及电子邮件等现代通信方式，同时参与的软件开发项目。Linux的开发模式是开放与协作的，在设计上融合了各方面的优点，也经历了各种各样的测试与考验。它具有一下特点：

- 开放与协作的开发模式。提供源代码，遵守GPL。	
- 发挥集体智慧，减少重复劳动。
- 经历了各种各样的测试与考验，软件的稳定性好。	
- 开发人员凭兴趣去开发，热情高，具有创造性。
