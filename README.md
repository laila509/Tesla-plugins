# 【分享】整合纯净的zdm65477730大佬终极版Tesla教程

Z大自从做了终极版Tesla，现在已经比原版还要好用，底座模式不死机，所有插件都兼容16.0和以上系统。莱莱强烈推荐。

因为不是每个人都需要全部的特斯拉插件，所以莱莱教大家怎么整合纯净版特斯拉包，有这个纯净包，小伙伴们可以在这基础上随意添加其它任何的ovl插件和启动器。

管理Tesla插件的确没有管理相册NRO软件那样直接替换一个nro那么简单，但是莱莱折腾Tesla以后并不觉得有什么门槛，都是很基础的折腾方法。

# 一，纯净Tesla的组件和原版下载地址

想玩Tesla插件，必定要有下面三个组件，其它的所有ovl插件都要基于这三个组件才能工作。

（1）nx-ovlloader，Tesla启动器

https://github.com/WerWolv/nx-ovlloader/releases

（2）ovlmenu，Tesla菜单

https://github.com/WerWolv/Tesla-Menu/releases

（3）ovlSysmodules，Tesla系统管理

https://github.com/WerWolv/ovl-sysmodules/releases

因为Z大佬基于这些插件做了优化编译

https://www.tekqart.com/thread-222735-1-1.html

https://github.com/zdm65477730

# 二，纯净Tesla的组件文件名和路径

（1）nx-ovlloader，Tesla启动器

路径在tf：atmosphere/contents/420000000007E51A/，其中

tf：atmosphere/contents/420000000007E51A/exefs.nsp，是Tesla启动器的核心文件

tf：atmosphere/contents/420000000007E51A/flags/boot2.flag，有boot2.flag文件=进系统自动启动

tf：atmospre/contents/420000000007E51A/toolbox.json，支持Deepsea工具箱开关插件的自动启动

（2）ovlmenu，Tesla菜单

有多个文件夹和文件，其中

tf：switch/.overlays/ovlmenu.ovl，是Tesla菜单的文件

tf：switch/.overlays/lang/TeslaMenu/，是Tesla菜单的多国语言包

tf：config/Tesla/config.ini，设定Tesla菜单的快捷键，没有就是默认的L+DDOWN+RS三键

tf：config/Tesla-Menu/sort.cfg，设定ovl插件上下排序，Z大编译的独特功能，和原版排序方法不一样

（3）ovlSysmodules，Tesla系统管理

有多个文件夹和文件，其中

tf：switch/.overlays/ovlsysmodules.ovl，Tesla系统管理的文件

tf：switch/.overlays/lang/Sysmodules/，是Tesla系统管理的多国语言包

tf：config/ovl-sysmodules/config.ini，是Tesla系统管理菜单里功能的显示和隐藏，建议显示

# 三，其它常用的ovl插件和路径

莱莱整合和搬运了Z大佬的终极版特斯拉，这里先教小伙伴们了解常用的ovl插件

（1）ovledizon，金手指插件

tf：switch/.overlays/edizon.ovl，是金手指插件ovl版本的文件，金手指码放在atmosphere/contents/

tf：switch/.overlays/lang/edizon/，是金手指软件ovl的多国语言包

tf：switch/EdiZon/EdiZon.nro，是金手指插件nro版本

（2）sys-clk-overlay，超频插件

tf：atmosphere/contents/00FF0000636C6BFF/，是超频插件的启动器，和Tesla启动器工作原理一样

其中00FF0000636C6BFF/exefs.nsp是超频插件启动器的核心文件

tf：config/sys-clk/config.ini，是超频插件设定文件，可删，有超频的ovl或nro都可以管理设定

tf：switch/.overlays/sys-clk.ovl，是超频插件管理器ovl版本

tf：switch/.overlays/lang/sys-clk/，是超频插件管理器ovl版本的多国语言包

tf：switch/sys-clk-manager.nro，是超频插件管理器nro版本

（3）ReverseNX-RT，手持底座切换插件

手持底座切换插件还包含了saltynx启动器和NX-FPS.elf两个组件

Status-Monitor-Overlay，系统监视器插件

这两个插件原版都由一位作者发布，而且系统监视器的实时FPS功能也要基于saltynx启动器才能工作

tf：atmosphere/contents/0000000000534C56/，是saltynx启动器，和Tesla启动器工作原理一样

其中0000000000534C56/exefs.nsp是saltynx启动器的核心文件

tf：switch/.overlays/ReverseNX-RT.ovl，是手持底座切换插件的文件，可以设定掌机下屏显主机分辨率

tf：switch/.overlays/lang/ReverseNX-RT/，是手持底座切换插件的多国语言包

tf：switch/.overlays/StatusMonitor.ovl，是系统监视器插件的文件

tf：switch/.overlays/lang/StatusMonitor/，是系统监视器插件的多国语言包

tf：SaltySD/，是手持底座切换插件的设定文件，其中

tf：SaltySD/plugins/NX-FPS.elf，是系统监视器的实时FPS功能的文件

tf：SaltySD/exceptions.txt，是因为部分游戏不支持手持底座切换容易出错，可编辑的免启动名单

（4）missioncontrol，支持蓝牙无线连接第三方手柄插件，这个插件只有启动器，无其它文件

tf：atmosphere/contents/010000000000bd00/，是missioncontrol启动器，和Tesla启动器工作原理一样

其中010000000000bd00/exefs.nsp是missioncontrol启动器的核心文件

tf：atmosphere/exefs_patches/bluetooth_patches，是missioncontrol适配SW系统的蓝牙补丁

tf：atmosphere/exefs_patches/btm_patches，新加的蓝牙补丁，适配15.0.0以后的系统

tf：config/MissionControl，missioncontrol设定文件，默认或删除都可以

（5）DeepSeaToolbox.nro，深海工具箱和Hekate，Kosmos工具箱一样，有管理启动器是否启动的功能

当删除420000000007E51A/flags/boot2.flag文件致Tesla菜单不能启动的时候，可以在这里开启且不用重启

这里还可以管理其它的启动器是否启动，这个和ovlSysmodules也提供一样的管理功能。

在后台管理各种启动器ON或者OFF后，要先按一次B键，再按一次Home键保存返回主界面，然后重启Switch。

# 四，更新的利器，Beyond Compare(文件对比工具)

Tesla以后也要跟着大气层和SW系统更新，所以首先更新核心组件，再更新其它的ovl插件，Beyond Compare(文件对比工具)来对比更新文件就非常简单

<img src="https://github.com/laila509/Tesla-plugins/blob/main/beyondcompare.jpg?raw=true?raw=true" align="center" width="80%" /> 
