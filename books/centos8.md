# centos8的优化记录

## 启动字符界面
通常安装的图形界面会占用较多内存，节省内存可以使用字符界面：

使用

        systemctl get-default
        
可以得知当前界面使用graphical.target

那么按照提示, 使用

        systemctl set-default multi-user.target

用这种方法仍然可以使用

        startx

命令启动图形界面。

## Liberoffice安装中文界面
由于操作系统层面用英文更通用一些，可避免终端乱码的问题，那么就要手动安装相应GUI软件的中文支持了，比如office工具要执行下面的命令后才能在tools中设定显示语言为中文，先查看相应的语言包：

        yum search libreoffice |grep -i han
        
再执行对应的安装：

        sudo yum install libreoffice-langpack-zh-Hans.x86_64
        
## 中文输入法的支持
要通过ibus来实现比较简单，可以快速安装google拼音与海峰五笔[跟王码86版较接近]。

