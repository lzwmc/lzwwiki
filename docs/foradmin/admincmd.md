## 原版指令
1、/op给予一位玩家管理员身份。

2、/deop撤销一位玩家的管理员身份。

3、/kick将一位玩家踢出服务器。

4、/pardon从黑名单移除项目。

5、/save-all将服务器保存至硬盘中。

6、/save-off禁用服务器自动保存。

7、/save-on启用服务器自动保存。

8、/scoreboard管理对象、玩家和队伍。

9、/setidletimeout设定踢出挂机玩家的时间。

10、/setworldspawn设定出生点。

11、/spawnpoint设定一位玩家的出生点。

12、/spreadplayers将实体传送至随机位置。

13、/stats通过命令的返回改变记分板对象。

14、/stop停止服务器。

15、/title管理屏幕标题。

16、/whitelist管理服务器白名单。

## htm
检查： /htm flag：敲击箱子检查容器是否公开 

设置： /htm set PUBLIC：敲击选择把容器设为公开。 

/htm set PRIVATE：运行命令后，敲击选择把容器设为私有，私有状态下只有你授权的玩家可以打开容器。 

/htm set KEY：运行命令后，拿着任意物品敲击容器，其他人打开容器时需使用敲击时的物品作为钥匙才能打开容器。 

信任和取消信任： /htm trust 玩家名 允许玩家打开你的容器。 

/htm untrust 玩家名 取消玩家打开你容器的权限。 

移除保护： /htm remove：移除该容器的保护 

转移权限： /htm transfer 玩家名：把敲击容器的保护权转移给其他玩家 

持续模式： /htm persist：打开后输入指令，即可一次敲击多个容器执行这个指令

## ledger
Inspect
/lg inspect - toggles inspect mode /lg inspect [on|off] - enables or disables inspect mode /lg inspect <pos> - inspects the block at a given position

Search
/lg search <args> - searches with the given arguments

Rollback
/lg rollback <args> - rollbacks with filters specified

Page
/lg page <index>
## InvView
- 指令：

    > 打开玩家背包：/view inv <玩家名>。

    > 打开玩家末影箱：/view echest <玩家名>。

- 权限：

    > invview.command.root：允许玩家使用“/view”指令。

    > invview.command.inv：允许玩家使用“/view inv”指令。

    > invview.command.echest：允许玩家使用“/view echest”指令。

    > invview.command.trinket：允许玩家使用“/view trinket”指令。

- invview.protected：允许玩家的背包不被其他人打开。

## Carpet
allowSpawningOfflinePlayers

Spawn offline players in online mode if online-mode player with specified name does not exist

    Type: Boolean
    Default value: true
    Required options: true, false
    Categories: COMMAND
    Additional notes:
        It has an accompanying command

antiCheatDisabled

Prevents players from rubberbanding when moving too fast
... or being kicked out for 'flying'
Puts more trust in clients positioning
Increases player allowed mining distance to 32 blocks

    Type: Boolean
    Default value: false
    Required options: true, false
    Categories: CREATIVE, SURVIVAL

carpetCommandPermissionLevel

Carpet command permission level. Can only be set via .conf file

    Type: String
    Default value: ops
    Required options: ops, 2, 4
    Categories: CREATIVE
    Additional notes:
        This setting can only be set by admins with op level 4

carpets

Placing carpets may issue carpet commands for non-op players

    Type: Boolean
    Default value: false
    Required options: true, false
    Categories: SURVIVAL

chainStone

Chains will stick to each other on the long ends
and will stick to other blocks that connect to them directly.
With stick_to_all: it will stick even if not visually connected

    Type: String
    Default value: false
    Required options: true, false, stick_to_all
    Categories: EXPERIMENTAL, FEATURE

cleanLogs

Removes obnoxious messages from the logs
Doesn't display 'Maximum sound pool size 247 reached'
Which is normal with decent farms and contraptions

    Type: Boolean
    Default value: false
    Required options: true, false
    Categories: SURVIVAL, CLIENT
    Additional notes:
        Its a client command so can be issued and potentially be effective when connecting to non-carpet/vanilla servers. In these situations (on vanilla servers) it will only affect the executing player, so each player needs to type it separately for the desired effect

commandDistance

Enables /distance command to measure in game distance between points
Also enables brown carpet placement action if 'carpets' rule is turned on as well

    Type: String
    Default value: true
    Required options: true, false, ops, 0, 1, 2, 3, 4
    Categories: COMMAND
    Additional notes:
        It has an accompanying command
        Can be limited to 'ops' only, true/false for everyone/no one, or a custom permission level

commandDraw

Enables /draw commands
... allows for drawing simple shapes or
other shapes which are sorta difficult to do normally

    Type: String
    Default value: ops
    Required options: true, false, ops, 0, 1, 2, 3, 4
    Categories: COMMAND
    Additional notes:
        It has an accompanying command
        Can be limited to 'ops' only, true/false for everyone/no one, or a custom permission level

commandInfo

Enables /info command for blocks
Also enables gray carpet placement action
if 'carpets' rule is turned on as well

    Type: String
    Default value: true
    Required options: true, false, ops, 0, 1, 2, 3, 4
    Categories: COMMAND
    Additional notes:
        It has an accompanying command
        Can be limited to 'ops' only, true/false for everyone/no one, or a custom permission level

commandLog

Enables /log command to monitor events via chat and overlays

    Type: String
    Default value: true
    Required options: true, false, ops, 0, 1, 2, 3, 4
    Categories: COMMAND
    Additional notes:
        It has an accompanying command
        Can be limited to 'ops' only, true/false for everyone/no one, or a custom permission level

commandPerimeterInfo

Enables /perimeterinfo command
... that scans the area around the block for potential spawnable spots

    Type: String
    Default value: true
    Required options: true, false, ops, 0, 1, 2, 3, 4
    Categories: COMMAND
    Additional notes:
        It has an accompanying command
        Can be limited to 'ops' only, true/false for everyone/no one, or a custom permission level

commandPlayer

Enables /player command to control/spawn players

    Type: String
    Default value: ops
    Required options: true, false, ops, 0, 1, 2, 3, 4
    Categories: COMMAND
    Additional notes:
        It has an accompanying command
        Can be limited to 'ops' only, true/false for everyone/no one, or a custom permission level

commandProfile

Enables /profile command to monitor game performance
subset of /tick command capabilities

    Type: String
    Default value: true
    Required options: true, false, ops, 0, 1, 2, 3, 4
    Categories: COMMAND
    Additional notes:
        It has an accompanying command
        Can be limited to 'ops' only, true/false for everyone/no one, or a custom permission level

commandScript

Enables /script command
An in-game scripting API for Scarpet programming language

    Type: String
    Default value: true
    Required options: true, false, ops, 0, 1, 2, 3, 4
    Categories: COMMAND, SCARPET
    Additional notes:
        It has an accompanying command
        Can be limited to 'ops' only, true/false for everyone/no one, or a custom permission level

commandScriptACE

Enables restrictions for arbitrary code execution with scarpet
Users that don't have this permission level
won't be able to load apps or /script run.
It is also the permission level apps will
have when running commands with run()

    Type: String
    Default value: ops
    Required options: ops, 0, 1, 2, 3, 4
    Categories: SCARPET
    Additional notes:
        Can be limited to 'ops' only, true/false for everyone/no one, or a custom permission level
        When changing the rule, you must at least have the permission level you are trying to give it

commandSpawn

Enables /spawn command for spawn tracking

    Type: String
    Default value: ops
    Required options: true, false, ops, 0, 1, 2, 3, 4
    Categories: COMMAND
    Additional notes:
        It has an accompanying command
        Can be limited to 'ops' only, true/false for everyone/no one, or a custom permission level

commandTick

Enables /tick command to control game clocks

    Type: String
    Default value: ops
    Required options: true, false, ops, 0, 1, 2, 3, 4
    Categories: COMMAND
    Additional notes:
        It has an accompanying command
        Can be limited to 'ops' only, true/false for everyone/no one, or a custom permission level

commandTrackAI

Allows to track mobs AI via /track command

    Type: String
    Default value: ops
    Required options: true, false, ops, 0, 1, 2, 3, 4
    Categories: COMMAND
    Additional notes:
        It has an accompanying command
        Can be limited to 'ops' only, true/false for everyone/no one, or a custom permission level

creativeFlyDrag

Creative air drag
Increased drag will slow down your flight
So need to adjust speed accordingly
With 1.0 drag, using speed of 11 seems to matching vanilla speeds.
Purely client side setting, meaning that
having it set on the decicated server has no effect
but this also means it will work on vanilla servers as well

    Type: Double
    Default value: 0.09
    Categories: CREATIVE, CLIENT
    Additional notes:
        Must be between 0 and 1
        Its a client command so can be issued and potentially be effective when connecting to non-carpet/vanilla servers. In these situations (on vanilla servers) it will only affect the executing player, so each player needs to type it separately for the desired effect

creativeFlySpeed

Creative flying speed multiplier
Purely client side setting, meaning that
having it set on the decicated server has no effect
but this also means it will work on vanilla servers as well

    Type: Double
    Default value: 1.0
    Categories: CREATIVE, CLIENT
    Additional notes:
        Must be a positive number or 0
        Its a client command so can be issued and potentially be effective when connecting to non-carpet/vanilla servers. In these situations (on vanilla servers) it will only affect the executing player, so each player needs to type it separately for the desired effect

creativeNoClip

Creative No Clip
On servers it needs to be set on both
client and server to function properly.
Has no effect when set on the server only
Can allow to phase through walls
if only set on the carpet client side
but requires some trapdoor magic to
allow the player to enter blocks

    Type: Boolean
    Default value: false
    Required options: true, false
    Categories: CREATIVE, CLIENT
    Additional notes:
        Its a client command so can be issued and potentially be effective when connecting to non-carpet/vanilla servers. In these situations (on vanilla servers) it will only affect the executing player, so each player needs to type it separately for the desired effect

creativePlayersLoadChunks

Creative players load chunks, or they don't! Just like spectators!
Toggling behaves exactly as if the player is in spectator mode and toggling the gamerule spectatorsGenerateChunks.

    Type: Boolean
    Default value: true
    Required options: true, false
    Categories: CREATIVE, FEATURE

ctrlQCraftingFix

Dropping entire stacks works also from on the crafting UI result slot

    Type: Boolean
    Default value: false
    Required options: true, false
    Categories: BUGFIX, SURVIVAL

customMOTD

Sets a different motd message on client trying to connect to the server
use '_' to use the startup setting from server.properties

    Type: String
    Default value: _
    Suggested options: _
    Categories: CREATIVE

defaultLoggers

sets these loggers in their default configurations for all new players
use csv, like 'tps,mobcaps' for multiple loggers, none for nothing

    Type: String
    Default value: none
    Suggested options: none, tps, mobcaps,tps
    Categories: CREATIVE, SURVIVAL

desertShrubs

Saplings turn into dead shrubs in hot climates and no water access

    Type: Boolean
    Default value: false
    Required options: true, false
    Categories: FEATURE

explosionNoBlockDamage

Explosions won't destroy blocks

    Type: Boolean
    Default value: false
    Required options: true, false
    Categories: CREATIVE, TNT

fastRedstoneDust

Lag optimizations for redstone dust
by Theosib
.. also fixes some locational behaviours or vanilla redstone MC-11193
so behaviour of locational vanilla contraptions is not guaranteed

    Type: Boolean
    Default value: false
    Required options: true, false
    Categories: EXPERIMENTAL, OPTIMIZATION

fillLimit

Customizable fill/clone volume limit

    Type: Integer
    Default value: 32768
    Suggested options: 32768, 250000, 1000000
    Categories: CREATIVE
    Additional notes:
        You must choose a value from 1 to 20M

fillUpdates

fill/clone/setblock and structure blocks cause block updates

    Type: Boolean
    Default value: true
    Required options: true, false
    Categories: CREATIVE

flatWorldStructureSpawning

Allows structure mobs to spawn in flat worlds

    Type: Boolean
    Default value: false
    Required options: true, false
    Categories: EXPERIMENTAL, CREATIVE

flippinCactus

Players can flip and rotate blocks when holding cactus
Doesn't cause block updates when rotated/flipped
Applies to pistons, observers, droppers, repeaters, stairs, glazed terracotta etc...

    Type: Boolean
    Default value: false
    Required options: true, false
    Categories: CREATIVE, SURVIVAL, FEATURE

fogOff

Removes fog from client in the nether and the end
Improves visibility, but looks weird

    Type: Boolean
    Default value: false
    Required options: true, false
    Categories: CLIENT
    Additional notes:
        Its a client command so can be issued and potentially be effective when connecting to non-carpet/vanilla servers. In these situations (on vanilla servers) it will only affect the executing player, so each player needs to type it separately for the desired effect

forceloadLimit

Customizable forceload chunk limit

    Type: Integer
    Default value: 256
    Suggested options: 256
    Categories: CREATIVE
    Additional notes:
        You must choose a value from 1 to 20M

hardcodeTNTangle

Sets the horizontal random angle on TNT for debugging of TNT contraptions
Set to -1 for default behavior

    Type: Double
    Default value: -1.0
    Suggested options: -1
    Categories: TNT
    Additional notes:
        Must be between 0 and 2pi, or -1

hopperCounters

hoppers pointing to wool will count items passing through them
Enables /counter command, and actions while placing red and green carpets on wool blocks
Use /counter <color?> reset to reset the counter, and /counter <color?> to query
In survival, place green carpet on same color wool to query, red to reset the counters
Counters are global and shared between players, 16 channels available
Items counted are destroyed, count up to one stack per tick per hopper

    Type: Boolean
    Default value: false
    Required options: true, false
    Categories: COMMAND, CREATIVE, FEATURE
    Additional notes:
        It has an accompanying command

huskSpawningInTemples

Only husks spawn in desert temples

    Type: Boolean
    Default value: false
    Required options: true, false
    Categories: FEATURE

interactionUpdates

placing blocks cause block updates

    Type: Boolean
    Default value: true
    Required options: true, false
    Categories: CREATIVE

lagFreeSpawning

Spawning requires much less CPU and Memory

    Type: Boolean
    Default value: false
    Required options: true, false
    Categories: OPTIMIZATION

language

Sets the language for Carpet

    Type: String
    Default value: en_us
    Required options: en_us, zh_cn, zh_tw
    Categories: FEATURE

leadFix

Fixes leads breaking/becoming invisible in unloaded chunks
You may still get visibly broken leash links on the client side, but server side the link is still there.

    Type: Boolean
    Default value: false
    Required options: true, false
    Categories: BUGFIX

lightEngineMaxBatchSize

Changes maximum light tasks batch size
Allows for a higher light suppression tolerance
setting it to 5 - Default limit defined by the game

    Type: Integer
    Default value: 5
    Suggested options: 5, 50, 100, 200
    Categories: EXPERIMENTAL, OPTIMIZATION

lightningKillsDropsFix

Lightning kills the items that drop when lightning kills an entity
Setting to true will prevent lightning from killing drops
Fixes MC-206922.

    Type: Boolean
    Default value: false
    Required options: true, false
    Categories: BUGFIX

liquidDamageDisabled

Disables breaking of blocks caused by flowing liquids

    Type: Boolean
    Default value: false
    Required options: true, false
    Categories: CREATIVE

maxEntityCollisions

Customizable maximal entity collision limits, 0 for no limits

    Type: Integer
    Default value: 0
    Suggested options: 0, 1, 20
    Categories: OPTIMIZATION
    Additional notes:
        Must be a positive number or 0

mergeTNT

Merges stationary primed TNT entities

    Type: Boolean
    Default value: false
    Required options: true, false
    Categories: TNT

missingTools

Glass can be broken faster with pickaxes

    Type: Boolean
    Default value: false
    Required options: true, false
    Categories: SURVIVAL

moreBlueSkulls

Increases for testing purposes number of blue skulls shot by the wither

    Type: Boolean
    Default value: false
    Required options: true, false
    Categories: CREATIVE

movableAmethyst

Allows Budding Amethyst blocks to be moved
Allow for them to be moved by pistons
as well as adds extra drop when mining with silk touch pickaxe

    Type: Boolean
    Default value: false
    Required options: true, false
    Categories: FEATURE

movableBlockEntities

Pistons can push block entities, like hoppers, chests etc.

    Type: Boolean
    Default value: false
    Required options: true, false
    Categories: EXPERIMENTAL, FEATURE

optimizedTNT

TNT causes less lag when exploding in the same spot and in liquids

    Type: Boolean
    Default value: false
    Required options: true, false
    Categories: TNT

perfPermissionLevel

Required permission level for /perf command

    Type: Integer
    Default value: 4
    Required options: 2, 4
    Categories: CREATIVE

persistentParrots

Parrots don't get of your shoulders until you receive proper damage

    Type: Boolean
    Default value: false
    Required options: true, false
    Categories: SURVIVAL, FEATURE

piglinsSpawningInBastions

Piglins will respawn in bastion remnants
Includes piglins, brutes, and a few hoglins

    Type: Boolean
    Default value: false
    Required options: true, false
    Categories: FEATURE

pingPlayerListLimit

Customizable server list ping (Multiplayer menu) playerlist sample limit

    Type: Integer
    Default value: 12
    Suggested options: 0, 12, 20, 40
    Categories: CREATIVE
    Additional notes:
        Must be a positive number or 0

placementRotationFix

fixes block placement rotation issue when player rotates quickly while placing blocks

    Type: Boolean
    Default value: false
    Required options: true, false
    Categories: BUGFIX

portalCreativeDelay

Amount of delay ticks to use a nether portal in creative

    Type: Integer
    Default value: 1
    Suggested options: 1, 40, 80, 72000
    Categories: CREATIVE
    Additional notes:
        You must choose a value from 1 to 72000

portalSurvivalDelay

Amount of delay ticks to use a nether portal in survival

    Type: Integer
    Default value: 80
    Suggested options: 1, 40, 80, 72000
    Categories: SURVIVAL
    Additional notes:
        You must choose a value from 1 to 72000

pushLimit

Customizable piston push limit

    Type: Integer
    Default value: 12
    Suggested options: 10, 12, 14, 100
    Categories: CREATIVE
    Additional notes:
        You must choose a value from 1 to 1024

quasiConnectivity

Pistons, droppers and dispensers react if block above them is powered

    Type: Boolean
    Default value: true
    Required options: true, false
    Categories: CREATIVE

railPowerLimit

Customizable powered rail power range

    Type: Integer
    Default value: 9
    Suggested options: 9, 15, 30
    Categories: CREATIVE
    Additional notes:
        You must choose a value from 1 to 1024

renewableBlackstone

Nether basalt generator without soul sand below
.. will convert into blackstone instead

    Type: Boolean
    Default value: false
    Required options: true, false
    Categories: FEATURE

renewableCoral

Coral structures will grow with bonemeal from coral plants
Expanded also allows growing from coral fans for sustainable farming outside of warm oceans

    Type: RenewableCoralMode
    Default value: false
    Required options: false, expanded, true
    Categories: FEATURE

renewableDeepslate

Lava and water generate deepslate and cobbled deepslate instead below Y0

    Type: Boolean
    Default value: false
    Required options: true, false
    Categories: FEATURE

renewableSponges

Guardians turn into Elder Guardian when struck by lightning

    Type: Boolean
    Default value: false
    Required options: true, false
    Categories: FEATURE

rotatorBlock

Cactus in dispensers rotates blocks.
Rotates block anti-clockwise if possible

    Type: Boolean
    Default value: false
    Required options: true, false
    Categories: FEATURE, DISPENSER

scriptsAppStore

Location of the online repository of scarpet apps
set to 'none' to disable.
Point to any github repo with scarpet apps
using //contents/<path...\>

    Type: String
    Default value: gnembon/scarpet/contents/programs
    Categories: SCARPET
    Additional notes:
        Appstore link should point to a valid github repository

scriptsAutoload

Scarpet script from world files will autoload on server/world start
if /script is enabled

    Type: Boolean
    Default value: true
    Required options: true, false
    Categories: SCARPET

scriptsDebugging

Enables scripts debugging messages in system log

    Type: Boolean
    Default value: false
    Required options: true, false
    Categories: SCARPET

scriptsOptimization

Enables scripts optimization

    Type: Boolean
    Default value: true
    Required options: true, false
    Categories: SCARPET

sculkSensorRange

Customizable sculk sensor range

    Type: Integer
    Default value: 8
    Suggested options: 8, 16, 32
    Categories: CREATIVE
    Additional notes:
        You must choose a value from 1 to 1024

shulkerSpawningInEndCities

Shulkers will respawn in end cities

    Type: Boolean
    Default value: false
    Required options: true, false
    Categories: FEATURE

silverFishDropGravel

Silverfish drop a gravel item when breaking out of a block

    Type: Boolean
    Default value: false
    Required options: true, false
    Categories: FEATURE

simulationDistance

Changes the simulation distance of the server.
Set to 0 to not override the value in server settings.

    Type: Integer
    Default value: 0
    Suggested options: 0, 12, 16, 32
    Categories: CREATIVE
    Additional notes:
        You must choose a value from 0 (use server settings) to 32

smoothClientAnimations

smooth client animations with low tps settings
works only in SP, and will slow down players

    Type: Boolean
    Default value: false
    Required options: true, false
    Categories: CREATIVE, SURVIVAL, CLIENT
    Additional notes:
        Its a client command so can be issued and potentially be effective when connecting to non-carpet/vanilla servers. In these situations (on vanilla servers) it will only affect the executing player, so each player needs to type it separately for the desired effect

spawnChunksSize

Changes size of spawn chunks
Defines new radius
setting it to 0 - disables spawn chunks

    Type: Integer
    Default value: 11
    Suggested options: 0, 11
    Categories: CREATIVE

stackableShulkerBoxes

Empty shulker boxes can stack when thrown on the ground.
.. or when manipulated inside the inventories

    Type: String
    Default value: false
    Suggested options: false, true, 16
    Categories: SURVIVAL, FEATURE
    Additional notes:
        Value must either be true, false, or a number between 2-64

structureBlockIgnored

Changes the block ignored by the Structure Block

    Type: String
    Default value: minecraft:structure_void
    Suggested options: minecraft:structure_void, minecraft:air
    Categories: CREATIVE

structureBlockLimit

Customizable structure block limit of each axis
WARNING: Needs to be permanent for correct loading.
Setting 'structureBlockIgnored' to air is recommended
when saving massive structures.
Required on client of player editing the Structure Block.
'structureBlockOutlineDistance' may be required for
correct rendering of long structures.

    Type: Integer
    Default value: 48
    Suggested options: 48, 96, 192, 256
    Categories: CREATIVE
    Additional notes:
        You have to choose a value greater or equal to 48

structureBlockOutlineDistance

Customizable Structure Block outline render distance
Required on client to work properly

    Type: Integer
    Default value: 96
    Suggested options: 96, 192, 2048
    Categories: CREATIVE, CLIENT
    Additional notes:
        Must be a positive number or 0
        Its a client command so can be issued and potentially be effective when connecting to non-carpet/vanilla servers. In these situations (on vanilla servers) it will only affect the executing player, so each player needs to type it separately for the desired effect

summonNaturalLightning

summoning a lightning bolt has all the side effects of natural lightning

    Type: Boolean
    Default value: false
    Required options: true, false
    Categories: CREATIVE

superSecretSetting

Gbhs sgnf sadsgras fhskdpri!!!

    Type: Boolean
    Default value: false
    Required options: true, false
    Categories: EXPERIMENTAL

tntDoNotUpdate

TNT doesn't update when placed against a power source

    Type: Boolean
    Default value: false
    Required options: true, false
    Categories: CREATIVE, TNT

tntPrimerMomentumRemoved

Removes random TNT momentum when primed

    Type: Boolean
    Default value: false
    Required options: true, false
    Categories: CREATIVE, TNT

tntRandomRange

Sets the tnt random explosion range to a fixed value
Set to -1 for default behavior

    Type: Double
    Default value: -1.0
    Suggested options: -1
    Categories: TNT
    Additional notes:
        optimizedTNT must be enabled
        Cannot be negative, except for -1

updateSuppressionBlock

Placing an activator rail on top of a barrier block will fill the neighbor updater stack when the rail turns off.
The integer entered is the amount of updates that should be left in the stack
-1 turns it off

    Type: Integer
    Default value: -1
    Suggested options: -1, 0, 10, 50
    Categories: CREATIVE
    Additional notes:
        This value represents the amount of updates required before the logger logs them. Must be -1 or larger

viewDistance

Changes the view distance of the server.
Set to 0 to not override the value in server settings.

    Type: Integer
    Default value: 0
    Suggested options: 0, 12, 16, 32
    Categories: CREATIVE
    Additional notes:
        You must choose a value from 0 (use server settings) to 32

xpFromExplosions

Experience will drop from all experience barring blocks with any explosion type

    Type: Boolean
    Default value: false
    Required options: true, false
    Categories: SURVIVAL, FEATURE

xpNoCooldown

Players absorb XP instantly, without delay

    Type: Boolean
    Default value: false
    Required options: true, false
    Categories: CREATIVE

## LuckPrems
/lpb (群组服务器主命令)

/lp  (子服务器主命令)

LuckPrems的子命令[用法](https://luckperms.net/wiki/Web-Editor)

## BungeeCord
提示：以下命令中<>尖括号内的参数为必填参数，[ ]方括号内的参数为选填参数

/alert <信息>

权限节点：bungeecord.command.alert

用途：发送一条整个群组的公告，会显示在所有的子服务器内。颜色符是&，使用&h 可以清除所有默认的格式

默认使用者：群组管理员

/alertraw <json格式的信息\>

权限节点：bungeecord.command.alert

用途：和上一个命令一样，但是仅允许使用json格式的内容

默认使用者：群组管理员

/bungee

权限节点：无

用途：显示BungeeCord的版本信息

默认使用者：所有玩家

/end

权限节点：bungeecord.command.end

用途：关闭BungeeCord代理端，类似于Bukkit服务器下的/stop

默认使用者：群组管理员

/find <玩家名>

权限节点：bungeecord.command.find

用途：确认指定玩家是否在线和他现在在哪个子服务器内

默认使用者：群组管理员

/glist

权限节点：bungeecord.command.list

用途：显示所有的子服务器和每个服务器当前在线人数

默认使用者：所有玩家

/greload

权限节点：bungeecord.command.reload

用途：重载BungeeCord代理端的配置文件，将重新载入子服务器列表、监听选项和一些配置项目，但是不会重载BC端插件和权限

默认使用者：群组管理员

/ip <玩家名>

权限节点：bungeecord.command.ip

用途：查看指定玩家的真实连接IP

默认使用者：群组管理员

/perms

权限节点：无

用途：显示你拥有的权限和所在权限组

默认使用者：所有玩家

/send <玩家名/current/all> <目标子服务器名>

权限节点：bungeecord.command.send

用途：将指定玩家移动到目标子服务器，使用“current”将会把你所在服务器的所有玩家移动到目标服务器，使用“all”将会把整个群组下的玩家移动到目标服务器。子服务器名就是你在“config.yml”的“servers”下面设置的服务器名

默认使用者：群组管理员

/server [子服务器名]

权限节点：bungeecord.command.server

用途：传送到指定子服务器，这个权限默认是高于Bukkit插件权限的，也就是说玩家可以在未登录之前使用此命令跳转到另外一个服务器，如果另外的服务器没登陆插件，那么通过此方法就可以使用到OP账号

默认使用者：所有玩家
