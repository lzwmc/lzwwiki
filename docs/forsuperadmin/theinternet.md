## 总体结构
本服务共若干台 分别负责用户的外置登录和游戏服务器，此外还有其他服务器

1. 外置登录，[101.43.228.112]，lazyworld.top

2. 游戏服务器，[112.255.86.24]，game.lazyworld.top

3. 服务器官网，[动态]，www.lazyworld.top

4. 邮箱服务器，[动态]，mail.lazywold.top

## 游戏服务器
游戏服务器中共若干个服务器端，负责玩家的游戏服务

| 名称 | 端口 | 外网是否可访问 | 登陆验证 | 连接方式 |
| :--: | :--: | :--: | :--: | :--: |
| 主服务器(生存服务器) | 25577 | 否 | 离线 | TCP |
| 群组服务器 | 25565 | 是 | 外置 | TCP |
| 基岩互通(作为群组服务器的插件) | 19132 | 是 | 离线 | UDP |

> 此外还有一些小游戏服务器从25577端口后延

## 服务器官网
托管到github上

## 邮箱服务器
支持协议:

1. SMTP
2. POP3
3. IMAP

> 均无SSL

## 外置登录
采用 [Blessing Skin Server](https://github.com/bs-community/blessing-skin-server) 搭建

### Blessing Skin
- 版本 	6.0.2
- 应用环境 	production
- 是否处于调试状态 	No

### Web服务软件
- Laravel 版本 	8.75.0
- 服务器
- PHP 版本 	8.0.21
- Web 服务软件 	nginx/1.21.1
- 操作系统 	Windows NT 10.0 AMD64

### 数据库
- 服务器类型 	MySQL/MariaDB
- 主机 	localhost
- 端口 	3306
- 用户名 	username
- 数据库 	blessingskin

### 插件
- Yggdrasil API 	5.1.5

