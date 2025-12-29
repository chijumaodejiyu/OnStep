OnStep 望远镜控制器
===========================
# 重要说明

OnStep 有多个 GitHub 分支：
* **发布分支** 经过充分测试，是大多数用户应该使用的版本。通常推荐使用最新的（修订版本最高的）发布版本。这些分支不会添加新功能，只会在必要时进行安全修复。
* **测试版分支**（如果存在）是主分支的"快照"，在我们达到相对稳定状态时创建。这为喜欢冒险的用户提供了大多数新功能的访问权限。
* **主分支** 是最新的 OnStep 版本，新功能在此添加。这是测试最不充分的分支，只应由有经验的用户使用，愿意测试并报告错误。

# 什么是 OnStep？
OnStep 是一个计算机化的望远镜 GOTO 控制器，基于 Teensy 或 Arduino 控制步进电机。

它支持赤道仪（GEM、叉式等）以及地平式支架（包括道布森式等）。

OnStep 从一开始就被设计为一个通用系统，固件中预留了在各种支架上使用的功能。

# 功能特性
OnStep 支持多种连接选项。可以使用两个或三个串行"命令通道"。其中一个通常用于 USB 连接，其他通道可以从以下选项中选择：

* 蓝牙
* ESP8266 WiFi
* Arduino M0/以太网扩展板
* 甚至添加另一个 USB 端口或 RS232 串口也不难。

OnStep 生态系统中的其他软件包括：

* [ASCOM](http://ascom-standards.org/) 驱动程序（支持 IP 和串行连接）
* 可通过 WiFi 或蓝牙连接的 Android 应用（版本 2.3.3 或更高）
* "内置"网站（在以太网和/或 WiFi 设备上）
* 控制所有功能的完整天文馆程序（[Sky Planetarium](http://stellarjourney.com/index.php?r=site/software_sky)）

OnStep 兼容 LX200 协议。这意味着它可以被其他天文馆软件控制，如：Sky Safari、CdC（即使没有 ASCOM）、Stellarium 等。

还有 [INDI](http://www.indilib.org/about.html) 驱动程序，因此可以在 Linux 上与 CdC 或 KStars 一起使用。

# 文档
详细的文档，包括完整的功能集、PCB 的详细设计、如何构建控制器的说明、如何为特定支架配置固件等，都可以在 [OnStep Group Wiki](https://groups.io/g/onstep/wiki/home) 中找到。

# 变更日志
所有变更都在 git 中跟踪，可以使用以下 git 命令查看详细列表：
 
git log --date=short --pretty=format:"%h %ad %<(20)%an %<(150,trunc)%s"

# 支持
问题和讨论应在邮件列表（也可通过网页访问）中进行：[OnStep Group](https://groups.io/g/onstep/)。

# 许可证
OnStep 是开源免费软件，采用 GPL 许可证。

请参阅 [LICENSE.txt](./LICENSE.txt) 文件。

# 作者
[Howard Dutton](http://www.stellarjourney.com)
