# Linux简介

[TOC]

Linux 是一套开放源代码程序的、可以自由传播的**类 Unix** 操作系统软件。

Linux 在设计之初，就是**基于 Intel x86 系列 CPU 架构**计算机的，它是一个**基于 POSIX** 的多用户、多任务并且支持多线程和多 CPU 的操作系统。

### Linux和UNIX的关系及区别：

Windows 和 Linux 都参考了 UNIX。

UNIX 操作系统由肯•汤普森（Ken Thompson）和丹尼斯•里奇（Dennis Ritchie）发明。

美国国防部把 TCP/IP 协议与 UNIX 系统、C语言捆绑在一起，由 AT&T 发行给美国各个大学非商业的许可证，这为 **UNIX 系统**、**C语言**、**TCP/IP 协议**的发展拉开了序幕，它们分别在操作系统、编程语言、网络协议这三个领域影响至今。

**Solaris** 是 UNIX 系统的一个重要分支。Solaris 除可以运行在 SPARC CPU 平台上外，还可以运行在 x86 CPU 平台上。**FreeBSD** 源于美国加利福尼亚大学伯克利分校开发的 UNIX 版本。FreeBSD 在 **BSD 许可协议**下发布，允许任何人在保留版权和许可协议信息的前提下随意使用和发行，并不限制将 FreeBSD 的代码在另一协议下发行。

Linux 内核最初是由**李纳斯•托瓦兹（Linus Torvalds）**在赫尔辛基大学读书时出于个人爱好而编写的。

据估计，现在只有 2% 的 Linux 核心代码是由李纳斯•托瓦兹自己编写的，虽然他仍然拥有 Linux 内核（操作系统的核心部分），并且保留了选择新代码和需要合并的新方法的最终裁定权。

#### 二者区别

1. **UNIX 系统大多是与硬件配套的**，也就是说，大多数 UNIX 系统如 AIX、HP-UX 等是无法安装在 x86 服务器和个人计算机上的，而 Linux 则可以运行在多种硬件平台上。
2. UNIX 是商业软件，而 Linux 是开源软件，是免费、公开源代码的。

### UNIX/Linux系统结构

#### 内核层

内核层是 UNIX/Linux 系统的核心和基础，它直接附着在硬件平台之上，控制和管理系统内各种资源（硬件资源和软件资源），有效地组织进程的运行，从而扩展硬件的功能，提高资源的利用效率，为用户提供方便、高效、安全、可靠的应用环境。

#### Shell层

**Shell 层是与用户直接交互的界面。**用户可以在提示符下输入命令行，由 Shell 解释执行并输出相应结果或者有关信息，所以我们也把 Shell 称作命令解释器，利用系统提供的丰富命令可以快捷而简便地完成许多工作。

#### 应用层

**应用层提供基于 X Window 协议的图形环境。**X Window 协议定义了一个系统所必须具备的功能（就如同 TCP/IP 是一个协议，定义软件所应具备的功能），系统能满足此协议及符合 X 协会其他的规范，便可称为 X Window。

### 常见Linux发行版本

从技术上来说，李纳斯•托瓦兹开发的 Linux 只是一个**内核**。内核指的是一个提供设备驱动、文件系统、进程管理、网络通信等功能的系统软件，内核并不是一套完整的操作系统，它只是操作系统的核心。

一些组织或厂商将 Linux 内核与各种软件和文档包装起来，并提供系统安装界面和系统配置、设定与管理工具，就构成了 Linux 的发行版本。

**Linux 发行版本大体分为两类：**

- **商业公司维护**的发行版本，以著名的 Red Hat 为代表。
- **社区组织维护**的发行版本，以 Debian 为代表。

#### Red Hat Linux

Red Hat（红帽公司）是目前世界上资深的 Linux 厂商，也是最获认可的 Linux 品牌。产品主要包括 **RHEL**（Red Hat Enterprise Linux，收费版本）和 **CentOS**（RHEL 的社区克隆版本，免费版本）、**Fedora Core**（由 Red Hat 桌面版发展而来，免费版本）。

#### Ubuntu Linux

Ubuntu 基于知名的 **Debian Linux** 发展而来，是目前最适合做桌面系统的 Linux 发行版本。

#### SuSE Linux

SuSE Linux 以 Slackware Linux 为基础，在欧洲较为流行，吸取了 Red Hat Linux 的很多特质。

**CentOS 是使用免费的 RHEL 的源代码重新编译而成的**，免费提供给大家，而且其本质上和 RHEL 没什么区别。国内多数企业使用 RHEL 搭建服务器，而且目前使用 CentOS 的企业越来越多。

### Linux桌面环境（桌面系统）

Linux 中的桌面环境也是一个程序，它和内核不是绑定的，两者的开发也不是同步的。

#### KDE 桌面系统

KDE 是 **K Desktop Environment** 的缩写，许多流行的 Linux 发行版都提供了 KDE 桌面环境，比如 Ubuntu、Linux Mint、OpenSUSE、Fedora、Kubuntu、PC Linux OS 等。

KDE 是所有桌面环境中最容易定制的。KDE 项目组还还发了大量的可运行在 KDE 环境中的应用程序，包括 Dolphin（文件管理工具）、Konsole（终端）、Kate（文本编辑工具）、Gwenview（图片查看工具）、Okular（文档及PDF查看工具）、Digikam（照片编辑和整理工具）、KMail（电子邮件客户软件）、Quassel（IRC客户软件）、K3b（DVD刻录程序）、Krunner（启动器）等，它们都是默认安装的。

#### GNOME 桌面环境

GNOME 是 **the GNU Network Object Model Environment** 的缩写，现已成为许多Linux发行版默认的桌面环境，用得最多的是 Red Hat Linux。GNOME 的特点是简洁、运行速度快，但是没有太多的定制选项，用户需要安装第三方工具来实现。GNOME 被用作 Fedora 中的默认桌面环境，提供在几款流行的 Linux 发行版中，比如 Ubuntu、Debian、OpenSUSE 等。

#### Unity

Unity 是由 Ubuntu 的母公司 Canonical 开发的一款外壳。之所以说它是外壳，是因为 Unity 运行在 GNOME 桌面环境之上，使用了所有 GNOME 的核心应用程序。

#### MATE

MATE 是一种从现在无人维护的 **GNOME 2 代码库派生**出来的桌面环境。

#### Cinnamon

与 MATE 类似，Cinnamon 是由 Linux Mint 团队因为不满 Gnome 3 的改进而开发的另一种桌面环境。但 Cinnamon 与 MATE 不同之处在于，**Cinnamon 建立在 Gnome 3 的基础上。**

