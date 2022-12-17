## 服务器目录结构
> 本文会去除一些没有必要了解的文件和结构

```
C:.
│   authlib-injector-1.2.1.jar 外置登录
│   authlib-injector.log 日志
│   banned-ips.json ban的ip名单
│   banned-players.json ban的玩家名单
│   eula.txt 许可协议
│   fabric-installer-0.11.0.exe 安装包
│   fabric-server-launch.jar 服务器入口
│   fabric-server-launcher.properties 服务器版本设置
│   ops.json 管理员名单
│   run.bat 开启本服务器脚本
│   server.jar 服务器主脚本
│   server.properties 服务器设置
│   start.bat 开启脚本(自动开启群组服务器)
│   usercache.json 用户缓存
│   whitelist.json 白名单
├───.fabric
├───BungeeCord 群组服务器
│   │   authlib-injector-1.2.1.jar 外置登录
│   │   authlib-injector.log 日志
│   │   BungeeCord.jar 主脚本
│   │   config.yml 配置文件
│   │   fabric-server-launcher.properties 配置文件
│   │   locations.yml 用户地点文件
│   │   modules.yml 模块配置文件
│   │   proxy.log.0 日志
│   │   proxy.log.0.lck 日志锁定文件
│   │   run.bat 开启脚本
│   │   
│   ├───modules 模块(全默认)
│   │       cmd_alert.jar
│   │       cmd_find.jar
│   │       cmd_list.jar
│   │       cmd_send.jar
│   │       cmd_server.jar
│   │       reconnect_yaml.jar
│   │       
│   └───plugins 插件
│       │   BanCommandPlus-BungeeCord-v1.1.0.jar 屏蔽指令
│       │   floodgate-bungee.jar 对基岩采取不同的用户名
│       │   Geyser-BungeeCord.jar 基岩互通
│       │   LuckPerms-Bungee-5.4.52.jar 权限细分的群组版
│       │   
│       ├───BanCommandPlus (以下皆为配置文件)
│       │       config.yml
│       │       
│       ├───bStats
│       │       config.yml
│       │       temp.txt
│       │       
│       ├───floodgate
│       │       config.yml
│       │       key.pem
│       │       
│       ├───Geyser-BungeeCord
│       │   │   config.yml
│       │   │   
│       │   ├───custom_mappings
│       │   ├───extensions
│       │   ├───locales
│       │   │       zh_cn.json
│       │   │       
│       │   └───packs
│       └───LuckPerms
│           │   config.yml
│           │   contexts.json
│           │   luckperms-h2-v2.mv.db
│           ├───libs
├───config 主服务器配置文件
│   │   cardinal-components-api.properties
│   │   htm_config.json
│   │   ledger.toml
│   │   NoChatReports.json
│   │   
│   ├───carpettisaddition
│   ├───chunky
│   │   │   config.json
│   │   │   
│   │   └───tasks
│   │       └───minecraft
│   │               overworld.properties
│   │               
│   └───luckperms
│       │   luckperms.conf
│       │   
│       └───translations
│           ├───custom
│           └───repository
├───GameServer 子服务器文件夹(结构与主服务器类似)
├───libraries 运行时库
├───logs 日志
├───mods 模组
│   │   Chunky-1.3.50.jar.d 区块预加载
│   │   easyauth-mc1.19.1-3.0.0-8.jar.d 密码验证
│   │   fabric-carpet-1.19.1-1.4.83+v220727.jar 地毯模组
│   │   fabric-language-kotlin-1.8.6+kotlin.1.7.21.jar 支持kotlin语言
│   │   gugle-carpet-addition-2.5.0-1.19.jar 地毯附加
│   │   htm-1.1.6.jar 锁箱
│   │   InvView-1.4.9-1.19+.jar 查看背包
│   │   ledger-1.2.5.jar 防熊
│   │   LuckPerms-Fabric-5.4.49.jar 权限细分
│   │   portal_cubed-2.2.8.jar 
│   │   [FabricAPI]fabric-api-0.60.0+1.19.2.jar FabricAPI
|   |   (以下为地毯模组附加)
│   │   [地毯][PCA]plusls-carpet-addition-1.19.2-0.2.5-beta+827168a.jar PCA
│   │   [地毯][TIS附加]carpet-tis-addition-mc1.19.2-v1.39.0+build.1219.jar TIS附加
│   │   [地毯][扩展]carpet-extra-1.19.1-1.4.83.jar 扩展
│   ├───EasyAuth 配置文件
│   │   │   config.json
│   │   └───levelDBStore
│   └───luckperms 配置文件
│       │   contexts.json
│       │   luckperms-h2.mv.db
│       │   
│       └───libs
├───versions 服务器主脚本
│   └───1.19.2
│           server-1.19.2.jar
└───world 存档(世界目录遵循原版目录)
    │   carpet.conf 配置文件
    │   ledger.sqlite 数据库
    │   level.dat
    │   level.dat_old
    │   session.lock
    │   
    ├───advancements
    ├───data
    │   ├───poi
    │   └───region
    ├───DIM1
    │   ├───data
    │   │       raids_end.dat
    │   ├───entities
    │   ├───poi
    │   └───region
    ├───dimensions
    │   └───twilightforest
    │       └───twilight_forest
    │           └───data
    │                   raids.dat
    ├───entities
    ├───playerdata
    ├───poi
    ├───region
    ├───scripts
    ├───serverconfig
    └───stats
```