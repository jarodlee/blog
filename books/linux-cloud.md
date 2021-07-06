# Linux主机管理

## 面板软件的安装

```text
wget http://amh.sh/amh.sh && bash amh.sh acc 914
```

在登录后执行上面的命令就可以得到一个可以通过浏览器配置linux的面板,用IP:8888就可以访问,安装完成时也会有相应的用户名与密码提示.

如果当时没保存或者忘记了密码,也可以用SSH登录服务器执行命令

```text
amh amh-6.0 admin reset_amh_password new_pass
```

重置面板密码 \(new\_pass改成您需要的密码\)

