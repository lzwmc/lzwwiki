## 简述
Nginx (engine x) 是一个高性能的HTTP和反向代理web服务器

## 在本服务器上的使用方法
使用Putty链接到服务器上后
`cd /usr/local/nginx/`
就来到了nginx的根目录

其中`conf`文件夹是配置文件 其中的`nginx.conf`是最关键的配置文件

`nginx.conf`的配置方法为[【Nginx】之 nginx.conf 配置详解](https://blog.csdn.net/aiwangtingyun/article/details/118823582)

其中`sbin`文件夹是可执行文件 可以使用:
```
sudo ./nginx 启动nginx
sudo ./nginx -s reload 重载配置文件(在每次修改配置文件后需要来到sbin目录执行此命令)
sudo ./nginx -s stop 停止nginx服务
```