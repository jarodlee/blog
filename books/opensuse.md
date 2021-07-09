# openSuSe的优化记录

将使用opensuse的过程中做的一些重要问题加以记录。

## 科大的源
opensuse官方源国内访问有问题，只好换成了科大的源：

        https://mirrors.ustc.edu.cn/opensuse/tumbleweed/repo/oss/

可参考官方的一个[文档说明](https://zh.opensuse.org/SDB:%E6%B7%BB%E5%8A%A0%E8%BD%AF%E4%BB%B6%E6%BA%90#.E6.B7.BB.E5.8A.A0.E9.95.9C.E5.83.8F.E6.BA.90)

## 系统软件安装方法

opensuse的安装软件命令又不一样了，比如安装git要这样：

        zypper in git-core

## 中文的设置方式

在 Yast 的 Language 配置中将中文加入，可以把简体中文（Simplified Chinese）选择为第二语言（Secondary Language），确认之后，系统会自动下载语言相关的组件和字体，注销当前登录之后生效。不过我还是把中文设成主语言了。相应的其他功能都会自动到位，比如liboffice的中文界面，输入法什么的都很快安装好了。

## opensuse的支持网站

使用nvdia的显卡：https://en.opensuse.org/SDB:NVIDIA_drivers 不过我的电脑是集显的，就不测试这个了。

opensuse的版本非常多，免费个人用户直接用Leap版本就好了。各版本的发行状况都是公开的：https://build.opensuse.org/monitor

官方文档在这：https://doc.opensuse.org/ 有[中文版](https://doc.opensuse.org/zh-CN/)

## 安装atom

从官网下载rpm包直接安装是个简单快捷的办法：

      sudo rpm -ivh ./atom.x86_64.rpm

如果没有LSB会出错误：依赖检测失败：
    lsb-core-noarch 被 atom-1.57.0-0.1.x86_64 需要

LSB是linux基本包的缩写，有时候定制安装会没有选上，这就要费点事了，走合适的源安装补上就行了：https://software.opensuse.org/package/lsb?locale=zh_TW

## sshd服务默认没开
要用root帐号手动启动一下：

        systemctl start sshd

要开机自动启动sshd就要设置：

        systemctl enable sshd

参考：[国外的一个指导文档](https://www.cyberithub.com/how-to-start-and-enable-sshd-service-in-opensuse-linux/#:~:text=How%20to%20Enable%20SSHD%20Service%20on%20OpenSUSE%20Linux,to%20manually%20start%20the%20Service%20after%20every%20reboot)

## ssh出现能连接不能登录的问题
端口是正常的，可以连接，但输入正确密码也无法登录，原因不明，怀疑是当时在使用ssh的同时做了更新造成了什么冲突。
