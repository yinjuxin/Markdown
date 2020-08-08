# 虚拟机VMware 安装Mac Os10.14教程

VMware安装Windows和Linux比较类似，相对于今天要安装的MAC OS来说过程也比较简单。官方原版VMware是不支持MAC OS安装的，但是外国大神制作的解锁工具让VMware安装MAC OS成为了可能，让我们去看看具体怎么安装的吧！

**安装准备**：

1：VMware Workstation Pro v15.0.0

2：解锁工具Unlocker v3.0.0

3：macOS Mojave 10.14懒人版

**安装过程：**

1.关闭VMware ，打开任务管理器，并找到后台进程，右键-结束所有VMware的进程（带VMware的就是）。

![img](https://mmbiz.qpic.cn/mmbiz_png/kiciadc7CaaJ5N1gpIlReOOldZ7gQY8jmj70IlYibicHzrWgkLOtUV1UcR9np2ICicmvbFo7F9dkugJXJRxicmtNLIoA/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)

2.找到解锁工具，右键-以管理员身份运行win-install.cmd,脚本运行完毕会自动关闭。

<img src="https://mmbiz.qpic.cn/mmbiz_png/kiciadc7CaaJ5N1gpIlReOOldZ7gQY8jmjuLZvFVmrRhdXFYb5SQJOJPolfS86bfjUIv26yKYMm3CGySBJBuW67Q/640?wx_fmt=png&amp;tp=webp&amp;wxfrom=5&amp;wx_lazy=1&amp;wx_co=1" alt="img" style="zoom: 67%;" />

3.打开VMware，创建新的虚拟机，这次我选择“典型”。

<img src="https://mmbiz.qpic.cn/mmbiz_png/kiciadc7CaaJ5N1gpIlReOOldZ7gQY8jmjAUjzC6uT1HeQicCYpBv5Vsaf7VfXtnwtZ6s8icX23EXwjln91HZzeWCA/640?wx_fmt=png&amp;tp=webp&amp;wxfrom=5&amp;wx_lazy=1&amp;wx_co=1" alt="img" style="zoom: 80%;" />

4.安装来源是macOS Mojave 10.14懒人版文件，注意浏览的时候文件类型要选择所有文件，不然找不到macOS Mojave 10.14 18A391 Lazy Installer.cdr。

<img src="https://mmbiz.qpic.cn/mmbiz_png/kiciadc7CaaJ5N1gpIlReOOldZ7gQY8jmjticI1IG34TicLuJ4SfbXuReDRKGYDNmUnNKO4uc0nvJThicWRKZomSZCg/640?wx_fmt=png&amp;tp=webp&amp;wxfrom=5&amp;wx_lazy=1&amp;wx_co=1" alt="img" style="zoom:80%;" />

5.系统类型是MAC OS 10.14,如果没有以上的解锁操作，选项里是没有MAC OS可选的。

<img src="https://mmbiz.qpic.cn/mmbiz_png/kiciadc7CaaJ5N1gpIlReOOldZ7gQY8jmjbU8icxGVM52DSCIPiaK3suTDl0ibnH0dZ35LADibJpKzJzH4kWibtGgWwRw/640?wx_fmt=png&amp;tp=webp&amp;wxfrom=5&amp;wx_lazy=1&amp;wx_co=1" alt="img" style="zoom: 80%;" />

6.由于安装后系统文件会很大，我们要把默认的位置换成c盘以外的位置。

<img src="https://mmbiz.qpic.cn/mmbiz_png/kiciadc7CaaJ5N1gpIlReOOldZ7gQY8jmjDNQtgt1lsWuYDpibl3P8fCdDggA7hMdyKxicu3I46SyaBxrGaSuwLVqA/640?wx_fmt=png&amp;tp=webp&amp;wxfrom=5&amp;wx_lazy=1&amp;wx_co=1" alt="img" style="zoom:80%;" />

7. 以下的几步默认即可，如果后续觉得配置不够，可以自行调整，配置完毕，不要急着打开虚拟机，找到刚才虚拟机系统文件路径下的macOS 10.14.vmx，用记事本打开，在 smc.present = "TRUE" 后添加（smc.version = "0"）(建议您复制，不包括括号) 后保存。

<img src="https://mmbiz.qpic.cn/mmbiz_png/kiciadc7CaaJ5N1gpIlReOOldZ7gQY8jmjWVDuiczf5WIo7aqnjvW1zM9xuQic8c7u9IHiaOJ2q0ZeBrLeBhsdv0APQ/640?wx_fmt=png&amp;tp=webp&amp;wxfrom=5&amp;wx_lazy=1&amp;wx_co=1" alt="img" style="zoom:80%;" />

<img src="https://mmbiz.qpic.cn/mmbiz_png/kiciadc7CaaJ5N1gpIlReOOldZ7gQY8jmjAz1j0DI5RDbeNqrhJibzbULwADLRb5aZaHyySw8iafeQRuhTptwYib4mg/640?wx_fmt=png&amp;tp=webp&amp;wxfrom=5&amp;wx_lazy=1&amp;wx_co=1" alt="img" style="zoom:80%;" />

8.打开虚拟机，等待进度条加载完毕。

<img src="https://mmbiz.qpic.cn/mmbiz_png/kiciadc7CaaJ5N1gpIlReOOldZ7gQY8jmjiaQU0mnBJMEHjOKAjGzESsySicCEawkjwH0lcLQSRyyY17z7MWQU8BkQ/640?wx_fmt=png&amp;tp=webp&amp;wxfrom=5&amp;wx_lazy=1&amp;wx_co=1" alt="img" style="zoom:80%;" />

9.语言选择简体中文，同意条款，继续安装。

<img src="https://mmbiz.qpic.cn/mmbiz_png/kiciadc7CaaJ5N1gpIlReOOldZ7gQY8jmja3t1Qt7NVNjz4vnzQibJ7PMwx8UibvXWrzg7s2Kt72qRTJ6iaQbsOGVnw/640?wx_fmt=png&amp;tp=webp&amp;wxfrom=5&amp;wx_lazy=1&amp;wx_co=1" alt="img" style="zoom:80%;" />

<img src="https://mmbiz.qpic.cn/mmbiz_png/kiciadc7CaaJ5N1gpIlReOOldZ7gQY8jmjpgYI1JSK4bL3oroqqMPwxQJIkffbwGaxsruPrqLKz35Mrvpo3QK6wg/640?wx_fmt=png&amp;tp=webp&amp;wxfrom=5&amp;wx_lazy=1&amp;wx_co=1" alt="img" style="zoom:80%;" />

10.到这一步点击上方“实用工具”里的磁盘工具。

<img src="https://mmbiz.qpic.cn/mmbiz_png/kiciadc7CaaJ5N1gpIlReOOldZ7gQY8jmj7ibqXwo5FT9hicwiazBIjGryRdEibVvRyvQ7CfAc3SHibomG1ITI7SB5Y1g/640?wx_fmt=png&amp;tp=webp&amp;wxfrom=5&amp;wx_lazy=1&amp;wx_co=1" alt="img" style="zoom:80%;" />

11.单击左侧的vmware虚拟硬盘，然后找到上方的“编辑”-“抹掉”，名称就叫mac os吧。

<img src="https://mmbiz.qpic.cn/mmbiz_png/kiciadc7CaaJ5N1gpIlReOOldZ7gQY8jmjcrhYNQSRZns7peZQjMJUibyjPKFOPWBSCTU6OJXa2UmqTBr5sllgaqQ/640?wx_fmt=png&amp;tp=webp&amp;wxfrom=5&amp;wx_lazy=1&amp;wx_co=1" alt="img" style="zoom:80%;" />

<img src="https://mmbiz.qpic.cn/mmbiz_png/kiciadc7CaaJ5N1gpIlReOOldZ7gQY8jmjsG5BOzyIbzWxeQoqBTCxicxgZPkquNm2DhO60z0AHcPGNK9YzQfpxwA/640?wx_fmt=png&amp;tp=webp&amp;wxfrom=5&amp;wx_lazy=1&amp;wx_co=1" alt="img" style="zoom:80%;" />

12.关闭磁盘工具，右侧会多出我们刚才分出来的一个磁盘，选择这个磁盘并继续。

<img src="https://mmbiz.qpic.cn/mmbiz_png/kiciadc7CaaJ5N1gpIlReOOldZ7gQY8jmjI9GFtcMbpPYYhDhIJP2SfQPVvSqIrmEvoKToIElsHwVKic6cNDicXxqg/640?wx_fmt=png&amp;tp=webp&amp;wxfrom=5&amp;wx_lazy=1&amp;wx_co=1" alt="img" style="zoom:80%;" />

<img src="https://mmbiz.qpic.cn/mmbiz_png/kiciadc7CaaJ5N1gpIlReOOldZ7gQY8jmj2TyBbBzhoBWk00Vy2Rj0IsibA3k3r3WxcRYE33bvM3UUNG8H1L0oONg/640?wx_fmt=png&amp;tp=webp&amp;wxfrom=5&amp;wx_lazy=1&amp;wx_co=1" alt="img" style="zoom:80%;" />

13.待安装完成，国家选择中国，键盘选择简体中文，不传输信息，apple id稍后设置，创建用户名和密码。

<img src="https://mmbiz.qpic.cn/mmbiz_png/kiciadc7CaaJ5N1gpIlReOOldZ7gQY8jmjmCNiccm7yGibojK1HdIJqcyrPlTYFgp3XMwfXYg9ZKfuScslk95T7FOw/640?wx_fmt=png&amp;tp=webp&amp;wxfrom=5&amp;wx_lazy=1&amp;wx_co=1" alt="img" style="zoom:80%;" />

<img src="https://mmbiz.qpic.cn/mmbiz_png/kiciadc7CaaJ5N1gpIlReOOldZ7gQY8jmjqoVTmmwrELuPjdcapNeIarsOC4NtlxY6k0yDevobxTJaa5xiaibJGhicg/640?wx_fmt=png&amp;tp=webp&amp;wxfrom=5&amp;wx_lazy=1&amp;wx_co=1" alt="img" style="zoom:80%;" />

<img src="https://mmbiz.qpic.cn/mmbiz_png/kiciadc7CaaJ5N1gpIlReOOldZ7gQY8jmjKeia9yziaa6as41U4pA4cMvGweRf5QOtJPqNicBUeQGeXk0AjGfXcYSNA/640?wx_fmt=png&amp;tp=webp&amp;wxfrom=5&amp;wx_lazy=1&amp;wx_co=1" alt="img" style="zoom:80%;" />

<img src="https://mmbiz.qpic.cn/mmbiz_png/kiciadc7CaaJ5N1gpIlReOOldZ7gQY8jmjhrWOnLIPmLTlfknB5kcDNtEicibTK4f54ck0VbQQcOH1RJnKDxmYxXjg/640?wx_fmt=png&amp;tp=webp&amp;wxfrom=5&amp;wx_lazy=1&amp;wx_co=1" alt="img" style="zoom:80%;" />

14.全部设置完毕即可进入系统，首先推出安装磁盘，然后在vmware上方“虚拟机”选择安装vmware tools，安装完vmware tools重启系统即可实现全屏和文件共享功能（如果提示系统扩展被阻挡，请在偏好设置—安全与隐私中选择允许再次安装）。

<img src="https://mmbiz.qpic.cn/mmbiz_png/kiciadc7CaaJ5N1gpIlReOOldZ7gQY8jmjGxXSUDnokXOkOicaGdS5JGdo65sasKvuBDxvseWBnZ5zEN9I0K7TYQA/640?wx_fmt=png&amp;tp=webp&amp;wxfrom=5&amp;wx_lazy=1&amp;wx_co=1" alt="img" style="zoom:80%;" />

MacOS10.14懒人版镜像和虚拟机解锁工具在**百度云网盘-我的资源-黑苹果**中。