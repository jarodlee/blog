# 记录一下操作系统的使用感受

## windows
官方网站：https://www.microsoft.com/zh-hk/windows

### win7
官方网站：https://www.microsoft.com/en-us/software-download/windows7

这个版本已经停止维护，所以会出现一些很奇怪的问题，比如在访问一些重要网站时会提示https的证书问题，也基本上无解了。

#### 推荐指数
★★


### win10
官方网站：https://www.microsoftstore.com.cn/software/windows

#### 激活版
基本上跟正版的也就没什么区别了，特别是在选择优先体验版之后，新功能会自动更新，使用上也跟以前的windows习惯一致。

#### 推荐指数
★★★★

#### 未激活版
就是一个基本只能上网的工具软件了，很多新版主流软件，如VM，dreamware都不支持在无法更新的这个版本上安装。

#### 推荐指数
★

## linux
官方网站：https://www.linux.org/

### CentOS
官方网站：https://www.centos.org/

#### 体会
服务器大厂redhat的开源方案，在服务器领域是第一选择，跟redhat商业版也可以无缝对接，技术成长无限，但桌面端的使用会有一些不方便。

#### 推荐指数
★★★★

### ubuntu
官方网站：https://ubuntu.com/

#### 体会
非常主流一种桌面Linux解决方案，同时可以适应一部分的服务器需要，但是新版的snap软件安装方式会让强迫症们对df命令抓狂。。。。

#### 推荐指数
★★★★

### 深度
官方网站：https://www.deepin.org/zh/

#### 体会
一个几乎跟Ubuntu换皮一样的系统，好在内置的软件商店位于国内，软件的安装与更新速度较快，但系统资源的占用也很高，老旧的机器基本不要想正常使用了，除了在语言文字方面全中文化上有优势，实在看不出来有什么理由不使用原版的Ubuntu。

#### 推荐指数
★★★

### NOI Linux
官方网站： http://www.noi.cn

#### 体会
NOI复赛官方环境，集成了竞赛的编辑与评分软件，基于ubuntu14.04打造，内置源已经过期，需要手动修改。 配置国内源的方法参考此链接：https://zhangzj.github.io/2017/03/21/ubnutu-1404-ubuntu-source-list.html
    
apt源配置文件

    cd /etc/apt/ 

备份原来的 source.list 文件先 sudo source.list source.list.cp

接下来编辑文件，清空文件内容，我们会在 source.list.d 目录中添加分别的文件 sudo vi source.list

删除 source.list 内容，在目录 source.list.d 中新建 163.list 文件，插入以下内容：163源

    deb http://mirrors.163.com/ubuntu/ trusty main restricted universe multiverse
    
    deb http://mirrors.163.com/ubuntu/ trusty-security main restricted universe multiverse
    
    deb http://mirrors.163.com/ubuntu/ trusty-updates main restricted universe multiverse
    
    deb http://mirrors.163.com/ubuntu/ trusty-proposed main restricted universe multiverse
    
    deb http://mirrors.163.com/ubuntu/ trusty-backports main restricted universe multiverse
    
    deb-src http://mirrors.163.com/ubuntu/ trusty main restricted universe multiverse
    
    deb-src http://mirrors.163.com/ubuntu/ trusty-security main restricted universe multiverse
    
    deb-src http://mirrors.163.com/ubuntu/ trusty-updates main restricted universe multiverse
    
    deb-src http://mirrors.163.com/ubuntu/ trusty-proposed main restricted universe multiverse
    
    deb-src http://mirrors.163.com/ubuntu/ trusty-backports main restricted universe multiverse
    
或者使用阿里云源

    deb http://mirrors.aliyun.com/ubuntu/ trusty main restricted universe multiverse
    
    deb http://mirrors.aliyun.com/ubuntu/ trusty-security main restricted universe multiverse
    
    deb http://mirrors.aliyun.com/ubuntu/ trusty-updates main restricted universe multiverse
    
    deb http://mirrors.aliyun.com/ubuntu/ trusty-proposed main restricted universe multiverse
    
    deb http://mirrors.aliyun.com/ubuntu/ trusty-backports main restricted universe multiverse
    
    deb-src http://mirrors.aliyun.com/ubuntu/ trusty main restricted universe multiverse
    
    deb-src http://mirrors.aliyun.com/ubuntu/ trusty-security main restricted universe multiverse
    
    deb-src http://mirrors.aliyun.com/ubuntu/ trusty-updates main restricted universe multiverse
    
    deb-src http://mirrors.aliyun.com/ubuntu/ trusty-proposed main restricted universe multiverse
    
    deb-src http://mirrors.aliyun.com/ubuntu/ trusty-backports main restricted universe multiverse
    
更新软件包

    sudo apt update
    
    sudo apt upgrade
    
国内和国外的源速度不是一个级别的，嗖嗖的。

#### 推荐指数
★★
