## 服务器目录结构
```
├───.fabric
│   ├───processedMods
│   └───remappedJars
│       └───minecraft-1.19.2-0.14.9
├───BungeeCord
│   ├───modules
│   └───plugins
│       ├───BanCommandPlus
│       ├───bStats
│       ├───floodgate
│       ├───Geyser-BungeeCord
│       │   ├───custom_mappings
│       │   ├───extensions
│       │   ├───locales
│       │   └───packs
│       └───LuckPerms
│           ├───libs
│           └───translations
│               ├───custom
│               └───repository
├───config
│   ├───carpettisaddition
│   ├───chunky
│   │   └───tasks
│   │       └───minecraft
│   └───luckperms
│       └───translations
│           ├───custom
│           └───repository
├───debug
├───defaultconfigs
├───GameServer
│   ├───game2
│   │   ├───.fabric
│   │   │   ├───processedMods
│   │   │   └───remappedJars
│   │   │       └───minecraft-1.19.2-0.14.9
│   │   ├───libraries
│   │   │   ├───com
│   │   │   │   ├───github
│   │   │   │   │   └───oshi
│   │   │   │   │       └───oshi-core
│   │   │   │   │           └───5.8.5
│   │   │   │   ├───google
│   │   │   │   │   ├───code
│   │   │   │   │   │   └───gson
│   │   │   │   │   │       └───gson
│   │   │   │   │   │           └───2.8.9
│   │   │   │   │   └───guava
│   │   │   │   │       ├───failureaccess
│   │   │   │   │       │   └───1.0.1
│   │   │   │   │       └───guava
│   │   │   │   │           └───31.0.1-jre
│   │   │   │   └───mojang
│   │   │   │       ├───authlib
│   │   │   │       │   └───3.11.49
│   │   │   │       ├───brigadier
│   │   │   │       │   └───1.0.18
│   │   │   │       ├───datafixerupper
│   │   │   │       │   └───5.0.28
│   │   │   │       ├───javabridge
│   │   │   │       │   └───1.2.24
│   │   │   │       └───logging
│   │   │   │           └───1.0.0
│   │   │   ├───commons-io
│   │   │   │   └───commons-io
│   │   │   │       └───2.11.0
│   │   │   ├───io
│   │   │   │   └───netty
│   │   │   │       ├───netty-buffer
│   │   │   │       │   └───4.1.77.Final
│   │   │   │       ├───netty-codec
│   │   │   │       │   └───4.1.77.Final
│   │   │   │       ├───netty-common
│   │   │   │       │   └───4.1.77.Final
│   │   │   │       ├───netty-handler
│   │   │   │       │   └───4.1.77.Final
│   │   │   │       ├───netty-resolver
│   │   │   │       │   └───4.1.77.Final
│   │   │   │       ├───netty-transport
│   │   │   │       │   └───4.1.77.Final
│   │   │   │       ├───netty-transport-classes-epoll
│   │   │   │       │   └───4.1.77.Final
│   │   │   │       ├───netty-transport-native-epoll
│   │   │   │       │   └───4.1.77.Final
│   │   │   │       └───netty-transport-native-unix-common
│   │   │   │           └───4.1.77.Final
│   │   │   ├───it
│   │   │   │   └───unimi
│   │   │   │       └───dsi
│   │   │   │           └───fastutil
│   │   │   │               └───8.5.6
│   │   │   ├───net
│   │   │   │   ├───fabricmc
│   │   │   │   │   ├───access-widener
│   │   │   │   │   │   └───2.1.0
│   │   │   │   │   ├───fabric-loader
│   │   │   │   │   │   └───0.14.9
│   │   │   │   │   ├───intermediary
│   │   │   │   │   │   └───1.19.2
│   │   │   │   │   ├───sponge-mixin
│   │   │   │   │   │   └───0.11.4+mixin.0.8.5
│   │   │   │   │   ├───tiny-mappings-parser
│   │   │   │   │   │   └───0.3.0+build.17
│   │   │   │   │   └───tiny-remapper
│   │   │   │   │       └───0.8.2
│   │   │   │   ├───java
│   │   │   │   │   └───dev
│   │   │   │   │       └───jna
│   │   │   │   │           ├───jna
│   │   │   │   │           │   └───5.10.0
│   │   │   │   │           └───jna-platform
│   │   │   │   │               └───5.10.0
│   │   │   │   └───sf
│   │   │   │       └───jopt-simple
│   │   │   │           └───jopt-simple
│   │   │   │               └───5.0.4
│   │   │   └───org
│   │   │       ├───apache
│   │   │       │   ├───commons
│   │   │       │   │   └───commons-lang3
│   │   │       │   │       └───3.12.0
│   │   │       │   └───logging
│   │   │       │       └───log4j
│   │   │       │           ├───log4j-api
│   │   │       │           │   └───2.17.0
│   │   │       │           ├───log4j-core
│   │   │       │           │   └───2.17.0
│   │   │       │           └───log4j-slf4j18-impl
│   │   │       │               └───2.17.0
│   │   │       ├───ow2
│   │   │       │   └───asm
│   │   │       │       ├───asm
│   │   │       │       │   └───9.3
│   │   │       │       ├───asm-analysis
│   │   │       │       │   └───9.3
│   │   │       │       ├───asm-commons
│   │   │       │       │   └───9.3
│   │   │       │       ├───asm-tree
│   │   │       │       │   └───9.3
│   │   │       │       └───asm-util
│   │   │       │           └───9.3
│   │   │       └───slf4j
│   │   │           └───slf4j-api
│   │   │               └───1.8.0-beta4
│   │   ├───logs
│   │   ├───mods
│   │   ├───versions
│   │   │   └───1.19.2
│   │   └───world
│   │       ├───advancements
│   │       ├───data
│   │       ├───datapacks
│   │       │   ├───Bow Game Datapack
│   │       │   │   └───data
│   │       │   │       ├───bow_game
│   │       │   │       │   ├───functions
│   │       │   │       │   │   ├───gamemode_setup
│   │       │   │       │   │   ├───gamemode_update
│   │       │   │       │   │   ├───map_game_setup
│   │       │   │       │   │   └───map_update
│   │       │   │       │   └───predicates
│   │       │   │       └───minecraft
│   │       │   │           ├───advancements
│   │       │   │           │   ├───adventure
│   │       │   │           │   ├───end
│   │       │   │           │   ├───husbandry
│   │       │   │           │   ├───nether
│   │       │   │           │   └───story
│   │       │   │           └───tags
│   │       │   │               ├───blocks
│   │       │   │               │   └───mineable
│   │       │   │               ├───entity_types
│   │       │   │               ├───fluids
│   │       │   │               ├───functions
│   │       │   │               ├───game_events
│   │       │   │               ├───items
│   │       │   │               └───worldgen
│   │       │   │                   ├───biome
│   │       │   │                   │   └───has_structure
│   │       │   │                   └───configured_structure_
│   │       │   └───parkour
│   │       │       └───data
│   │       │           ├───main
│   │       │           │   ├───functions
│   │       │           │   │   ├───checkpoint
│   │       │           │   │   │   ├───display
│   │       │           │   │   │   ├───player
│   │       │           │   │   │   └───self
│   │       │           │   │   ├───items
│   │       │           │   │   ├───pb
│   │       │           │   │   │   ├───get_pb
│   │       │           │   │   │   └───store_pb
│   │       │           │   │   ├───services
│   │       │           │   │   │   └───fire
│   │       │           │   │   ├───timer
│   │       │           │   │   │   └───main
│   │       │           │   │   │       └───timer
│   │       │           │   │   ├───training_mode
│   │       │           │   │   │   ├───flight
│   │       │           │   │   │   └───save_pos
│   │       │           │   │   └───trigger
│   │       │           │   │       └───show_pb
│   │       │           │   ├───predicates
│   │       │           │   │   └───fire
│   │       │           │   └───tags
│   │       │           │       └───blocks
│   │       │           └───minecraft
│   │       │               ├───advancements
│   │       │               │   ├───adventure
│   │       │               │   ├───end
│   │       │               │   ├───husbandry
│   │       │               │   ├───nether
│   │       │               │   └───story
│   │       │               └───tags
│   │       │                   └───functions
│   │       ├───DIM-1
│   │       │   └───data
│   │       ├───DIM1
│   │       │   └───data
│   │       ├───entities
│   │       ├───playerdata
│   │       ├───poi
│   │       ├───region
│   │       ├───scripts
│   │       └───stats
│   └───paoku
│       ├───.fabric
│       │   ├───processedMods
│       │   └───remappedJars
│       │       └───minecraft-1.19.2-0.14.9
│       ├───libraries
│       │   ├───com
│       │   │   ├───github
│       │   │   │   └───oshi
│       │   │   │       └───oshi-core
│       │   │   │           └───5.8.5
│       │   │   ├───google
│       │   │   │   ├───code
│       │   │   │   │   └───gson
│       │   │   │   │       └───gson
│       │   │   │   │           └───2.8.9
│       │   │   │   └───guava
│       │   │   │       ├───failureaccess
│       │   │   │       │   └───1.0.1
│       │   │   │       └───guava
│       │   │   │           └───31.0.1-jre
│       │   │   └───mojang
│       │   │       ├───authlib
│       │   │       │   └───3.11.49
│       │   │       ├───brigadier
│       │   │       │   └───1.0.18
│       │   │       ├───datafixerupper
│       │   │       │   └───5.0.28
│       │   │       ├───javabridge
│       │   │       │   └───1.2.24
│       │   │       └───logging
│       │   │           └───1.0.0
│       │   ├───commons-io
│       │   │   └───commons-io
│       │   │       └───2.11.0
│       │   ├───io
│       │   │   └───netty
│       │   │       ├───netty-buffer
│       │   │       │   └───4.1.77.Final
│       │   │       ├───netty-codec
│       │   │       │   └───4.1.77.Final
│       │   │       ├───netty-common
│       │   │       │   └───4.1.77.Final
│       │   │       ├───netty-handler
│       │   │       │   └───4.1.77.Final
│       │   │       ├───netty-resolver
│       │   │       │   └───4.1.77.Final
│       │   │       ├───netty-transport
│       │   │       │   └───4.1.77.Final
│       │   │       ├───netty-transport-classes-epoll
│       │   │       │   └───4.1.77.Final
│       │   │       ├───netty-transport-native-epoll
│       │   │       │   └───4.1.77.Final
│       │   │       └───netty-transport-native-unix-common
│       │   │           └───4.1.77.Final
│       │   ├───it
│       │   │   └───unimi
│       │   │       └───dsi
│       │   │           └───fastutil
│       │   │               └───8.5.6
│       │   ├───net
│       │   │   ├───fabricmc
│       │   │   │   ├───access-widener
│       │   │   │   │   └───2.1.0
│       │   │   │   ├───fabric-loader
│       │   │   │   │   └───0.14.9
│       │   │   │   ├───intermediary
│       │   │   │   │   └───1.19.2
│       │   │   │   ├───sponge-mixin
│       │   │   │   │   └───0.11.4+mixin.0.8.5
│       │   │   │   ├───tiny-mappings-parser
│       │   │   │   │   └───0.3.0+build.17
│       │   │   │   └───tiny-remapper
│       │   │   │       └───0.8.2
│       │   │   ├───java
│       │   │   │   └───dev
│       │   │   │       └───jna
│       │   │   │           ├───jna
│       │   │   │           │   └───5.10.0
│       │   │   │           └───jna-platform
│       │   │   │               └───5.10.0
│       │   │   └───sf
│       │   │       └───jopt-simple
│       │   │           └───jopt-simple
│       │   │               └───5.0.4
│       │   └───org
│       │       ├───apache
│       │       │   ├───commons
│       │       │   │   └───commons-lang3
│       │       │   │       └───3.12.0
│       │       │   └───logging
│       │       │       └───log4j
│       │       │           ├───log4j-api
│       │       │           │   └───2.17.0
│       │       │           ├───log4j-core
│       │       │           │   └───2.17.0
│       │       │           └───log4j-slf4j18-impl
│       │       │               └───2.17.0
│       │       ├───ow2
│       │       │   └───asm
│       │       │       ├───asm
│       │       │       │   └───9.3
│       │       │       ├───asm-analysis
│       │       │       │   └───9.3
│       │       │       ├───asm-commons
│       │       │       │   └───9.3
│       │       │       ├───asm-tree
│       │       │       │   └───9.3
│       │       │       └───asm-util
│       │       │           └───9.3
│       │       └───slf4j
│       │           └───slf4j-api
│       │               └───1.8.0-beta4
│       ├───logs
│       ├───mods
│       ├───versions
│       │   └───1.19.2
│       └───world
│           ├───advancements
│           ├───data
│           ├───datapacks
│           │   └───parkour
│           │       └───data
│           │           ├───main
│           │           │   ├───functions
│           │           │   │   ├───checkpoint
│           │           │   │   │   ├───display
│           │           │   │   │   ├───player
│           │           │   │   │   └───self
│           │           │   │   ├───items
│           │           │   │   ├───pb
│           │           │   │   │   ├───get_pb
│           │           │   │   │   └───store_pb
│           │           │   │   ├───services
│           │           │   │   │   └───fire
│           │           │   │   ├───timer
│           │           │   │   │   └───main
│           │           │   │   │       └───timer
│           │           │   │   ├───training_mode
│           │           │   │   │   ├───flight
│           │           │   │   │   └───save_pos
│           │           │   │   └───trigger
│           │           │   │       └───show_pb
│           │           │   ├───predicates
│           │           │   │   └───fire
│           │           │   └───tags
│           │           │       └───blocks
│           │           └───minecraft
│           │               ├───advancements
│           │               │   ├───adventure
│           │               │   ├───end
│           │               │   ├───husbandry
│           │               │   ├───nether
│           │               │   └───story
│           │               └───tags
│           │                   └───functions
│           ├───DIM-1
│           │   └───data
│           ├───DIM1
│           │   └───data
│           ├───entities
│           ├───playerdata
│           ├───poi
│           ├───region
│           └───stats
├───libraries
│   ├───com
│   │   ├───github
│   │   │   └───oshi
│   │   │       └───oshi-core
│   │   │           └───5.8.5
│   │   ├───google
│   │   │   ├───code
│   │   │   │   └───gson
│   │   │   │       └───gson
│   │   │   │           └───2.8.9
│   │   │   └───guava
│   │   │       ├───failureaccess
│   │   │       │   └───1.0.1
│   │   │       └───guava
│   │   │           └───31.0.1-jre
│   │   └───mojang
│   │       ├───authlib
│   │       │   └───3.11.49
│   │       ├───brigadier
│   │       │   └───1.0.18
│   │       ├───datafixerupper
│   │       │   └───5.0.28
│   │       ├───javabridge
│   │       │   └───1.2.24
│   │       └───logging
│   │           └───1.0.0
│   ├───commons-io
│   │   └───commons-io
│   │       └───2.11.0
│   ├───io
│   │   └───netty
│   │       ├───netty-buffer
│   │       │   └───4.1.77.Final
│   │       ├───netty-codec
│   │       │   └───4.1.77.Final
│   │       ├───netty-common
│   │       │   └───4.1.77.Final
│   │       ├───netty-handler
│   │       │   └───4.1.77.Final
│   │       ├───netty-resolver
│   │       │   └───4.1.77.Final
│   │       ├───netty-transport
│   │       │   └───4.1.77.Final
│   │       ├───netty-transport-classes-epoll
│   │       │   └───4.1.77.Final
│   │       ├───netty-transport-native-epoll
│   │       │   └───4.1.77.Final
│   │       └───netty-transport-native-unix-common
│   │           └───4.1.77.Final
│   ├───it
│   │   └───unimi
│   │       └───dsi
│   │           └───fastutil
│   │               └───8.5.6
│   ├───net
│   │   ├───fabricmc
│   │   │   ├───access-widener
│   │   │   │   └───2.1.0
│   │   │   ├───fabric-loader
│   │   │   │   └───0.14.9
│   │   │   ├───intermediary
│   │   │   │   └───1.19.2
│   │   │   ├───sponge-mixin
│   │   │   │   └───0.11.4+mixin.0.8.5
│   │   │   ├───tiny-mappings-parser
│   │   │   │   └───0.3.0+build.17
│   │   │   └───tiny-remapper
│   │   │       └───0.8.2
│   │   ├───java
│   │   │   └───dev
│   │   │       └───jna
│   │   │           ├───jna
│   │   │           │   └───5.10.0
│   │   │           └───jna-platform
│   │   │               └───5.10.0
│   │   └───sf
│   │       └───jopt-simple
│   │           └───jopt-simple
│   │               └───5.0.4
│   └───org
│       ├───apache
│       │   ├───commons
│       │   │   └───commons-lang3
│       │   │       └───3.12.0
│       │   └───logging
│       │       └───log4j
│       │           ├───log4j-api
│       │           │   └───2.17.0
│       │           ├───log4j-core
│       │           │   └───2.17.0
│       │           └───log4j-slf4j18-impl
│       │               └───2.17.0
│       ├───ow2
│       │   └───asm
│       │       ├───asm
│       │       │   └───9.3
│       │       ├───asm-analysis
│       │       │   └───9.3
│       │       ├───asm-commons
│       │       │   └───9.3
│       │       ├───asm-tree
│       │       │   └───9.3
│       │       └───asm-util
│       │           └───9.3
│       └───slf4j
│           └───slf4j-api
│               └───1.8.0-beta4
├───logs
├───mods
│   ├───EasyAuth
│   │   └───levelDBStore
│   └───luckperms
│       └───libs
├───versions
│   └───1.19.2
└───world
    ├───advancements
    ├───data
    ├───datapacks
    ├───DIM-1
    │   ├───data
    │   ├───entities
    │   ├───poi
    │   └───region
    ├───DIM1
    │   ├───data
    │   ├───entities
    │   ├───poi
    │   └───region
    ├───dimensions
    │   └───twilightforest
    │       └───twilight_forest
    │           └───data
    ├───entities
    ├───playerdata
    ├───poi
    ├───region
    ├───scripts
    ├───serverconfig
    └───stats
```