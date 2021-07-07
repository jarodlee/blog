# centos8的优化记录

## 启动字符界面
通常安装的图形界面会占用较多内存，节省内存可以使用字符界面：

使用
        systemctl get-default
        
可以得知当前界面使用graphical.target

那么按照提示, 使用

        systemctl set-default multi-user.target