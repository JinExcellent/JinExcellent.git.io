## 个人信息

姓名：金志高

性别：男

邮箱：b110mrjin@gmail.com

专业：计算机科学与技术

Github：https://github.com/JinExcellent

## 专业技能

- 熟练使用C/C++（**OOP、泛编程、STL**），C++高级特性（**Lambd表达式、Function、智能指针、变参模板、模板折叠、万能引用和原样转发**）；
- 熟悉常用的几种单例模式（局部静态变量方式、裸指针方式-饿汉式、智能指针方式-懒汉式、通用单例模板类CRTP）；
- 熟练掌握计算机操作系统（**进程与线程、虚拟内存管理、文件系统管理**）；常用网络协议（**IP、ARP、DHCP、TCP/UDP、HTTP**）；计算机组成原理（数据表示、**Cache工作原理**、指令系统、数据通路、指令流水线、**异常和中断机制**、I/O通信）、数据结构（**二叉树、BFS、DFS、常用排序与查找算法**）的理论知识；
- 熟悉常用**X86**汇编指令；
- 熟悉常用的**POSIX**标准**系统编程**和**网络编程API**；
- 熟悉**linux**平台下的**开发工具链**：Vim、Ctags、Makefile、Shell、Git、Gcc、Nasm、Qemu、GDB（具备**多线程**和**Qemu裸机**调试的能力）；
- 会使用**MySQL**数据库语言
- 常通过国内外社区和论坛了解技术难题和最新技术动向，如**Stack Overflow**、Reddit、**OSdev**、OpenGroup等；

## 学习经历

- ##### 阅读过的技术书目

《C Primer Plus》《C++ Primer Plus》《C++ Primer》《Unix高级系统编程》《TCP/IP网络编程》《高性能服务器编程》《Unix网络编程》《Operating Systems: Three Easy Pieces》《程序员的自我修养》《深入设计模式》《鸟哥的Linux私房菜》

- #####  做过的一些练习

**线程安全智能指针**、实现Deque和map（使用普通二叉树）、**Unordermap**（使用哈希表）、学习**MIT6.1810**（XV6-RISC-V）

## 教育背景



## 项目经历

[微内核操作系统](https://github.com/JinExcellent/MakeOwnSystem) （技术栈：C、x86汇编、GDB、QEMU、Makefile、git、shell）

**项目简介**：参考书籍《30天自制操作系统》和OSdev论坛，在**Linux**平台下完成一个微内核操作系统，运行在x86架构下，在QEMU虚拟机上启动并调试。内核使用汇编和C语言编写，涵盖从Bootloader到多任务调度的完整操作系统核心模块。

主要工作：

- 实现 **Bootloader**，通过 BIOS 加载并初始化内核运行环境再从实模式切换到保护模式；
- 使用可编程中断控制器（PIC）配置硬件中断，构建**IDT**表和**GDT**表，设置中断服务入口与段描述符并加载到CPU，支持异常/外设中断处理与保护模式段式内存访问；
- **从0到1**实现鼠标绘制、中断事件处理，以及键盘字符输入、中断响应和字符显示;
- 开发 **内存管理** 模块：使用**动态内存分配技术**和**首次适应算法**进行物理内存分配，支持按页和动态大小分配;
- 实现**定时器**，使用”哨兵“等编程技巧来优化中断处理，从而解决中断和中断处理速度不匹配的问题
- 实现多任务管理，利用**TSS**保存任务上下文，使用**多级反馈队列MLFQ**实现多任务优先级调度，使用**管道**实现任务间通信
- 设计系统调用接口与用户交互机制，构建 **图形界面** 和基本窗口系统
- 使用 **QEMU + GDB** 进行内核远程调试，编写 Makefile 实现自动化构建流程

[轻量级WebServer服务器](https://github.com/JinExcellent/WebServe_test)  （技术栈：C/C++，POSIX API、网络编程API、MySQL、Makefile、git、Shell、GDB）

项目简介：参考书籍《高性能服务器编程》，

