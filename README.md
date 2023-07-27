# 设置
- 触控板
  - 辅助点按：双指点按或轻点
  - 轻点来点按：开启
- 辅助功能 -> 指针控制 -> 触控板选项
  - 使用触控板进行拖移：三指拖移
- 鼠标
    - 自然滚动：关闭

- 桌面与程序坞
  - 自动隐藏和显示菜单栏：仅在全屏幕视图下

# 软件
## 允许安装「任何来源」的应用程序
终端中输入：
```shell
sudo spctl --master-disable
```
然后 设置 -> 安全性与隐私 -> 安全性中勾选「任何来源」
## [Homewbrew](https://brew.sh/)

```shell
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```



## 常用软件

- 安装一栏中默认字符为 brew 中软件名，链接为安装包备份，空白为自行前往软件官网下载
- 备份

    - 参考链接：[macOS 使用 homebrew-bundle 优雅的备份和恢复软件列表 | HelloDog](https://wsgzao.github.io/post/homebrew-bundle/)

    - 备份(仅有brew 安装的软件，App Store 和第三方dmg安装未备份，[备份文件地址](https://github.com/insv23/MacOS/tree/main/brew_backup))

        ```shell
        brew bundle dump --describe --force --file="~/Documents/MacOS/brew_backup/Brewfile_2023-07-18"
        ```

    - 恢复

        ```shell
        brew bundle --file="~/Documents/MacOS/brew_backup/Brewfile_2023-07-18"
        ```

        


| 名字                                                         | 介绍                                                         | 价格                                                         | 安装                                                         | 替代品                                                       |
| :----------------------------------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| [Arc](https://arc.net/)                                      | 浏览器                                                       | 免费                                                         | arc                                                          |                                                              |
| [搜狗输入法](https://shurufa.sogou.com/)                     | 输入法  [配置](./SougouInputConfig.md)                       | 免费                                                         | sogouinput                                                   | [squirrel](https://baiyun.me/rime-simple-tutorial)           |
| [QSpace Pro](https://qspace.awehunt.com/en-us/index.html)    | 代替 Finder 的文件管理器                                     | ¥ 89 买断(已购)                                              | qspace-pro                                                   |                                                              |
| [AlDente](https://apphousekitchen.com/)                      | 手动控制电池充电限度                                         | 免费，[Pro](https://apphousekitchen.com/zh-hans/%e5%ae%9a%e4%bb%b7/) €11.30/年(未购) | aldente，[Pro安装包](https://github.com/insv23/MacOS/blob/main/installers/Aldente%20Pro%201.22_MacApp.dmg) |                                                              |
| [HapiGo](https://www.hapigo.com/)                            | 搜索、剪贴板、OCR、翻译、GPT                                 | 免费，Pro ¥69/年(已购)                                       |                                                              | [Alfred](https://github.com/insv23/MacOS/tree/main/installers/Alfred%205.0.5%20for%20Mac%20Powerpack) |
| [Keka](https://www.keka.io/en/)                              | 解压软件                                                     | 免费                                                         | keka                                                         |                                                              |
| [typora](https://typora.io/)                                 | markdown 编辑器                                              | $14.99 (3台设备)(已购)                                       | typora                                                       |                                                              |
| [Obsidian](https://obsidian.md/)                             | 第二大脑                                                     | 免费                                                         | obsidian                                                     |                                                              |
| [warp](https://www.warp.dev/)                                | 终端                                                         | 免费                                                         | warp                                                         | [fig](https://fig.io/)                                       |
| [Surge5](https://nssurge.com/)                               | 代理软件，[个人自定义配置使用指南](./SurgeConfig.md)         | ¥145 for Surge5大版本内终身(已购)                            | surge                                                        | [ClashX](https://github.com/yichengchen/clashX)              |
| [iShot](https://www.better365.cn/ishot.html)                 | 截图                                                         | ¥28/年(已购)                                                 |                                                              |                                                              |
| [Shottr](https://shottr.cc/)                                 | 截图软件，但打码标记等做的很好                               | 免费(可自愿购买 pro)                                         | shottr                                                       |                                                              |
| [Karabiner](https://karabiner-elements.pqrs.org/)            | 键盘改键([配置文件](https://github.com/insv23/MacOS/tree/main/configs/Karabiner)) | 免费                                                         | karabiner-elements                                           |                                                              |
| [腾讯柠檬](https://lemon.qq.com/)                            | 清理                                                         | 免费                                                         | tencent-lemon                                                |                                                              |
| [iStat Menus](https://bjango.com/mac/istatmenus/)            | 在菜单栏显示系统 CPU, Memory, SSD, 网速等状态                | $14.27                                                       | [安装包备份](https://github.com/insv23/MacOS/tree/main/installers/iStat%20Menus%206.70) |                                                              |
| [SoundSource](https://rogueamoeba.com/soundsource/)          | 在菜单栏直接选择音频输出设备，~~无法习惯新版 MacOS 引入 iOS 的控制中心的逻辑~~(可以拖拽控制中心的"声音"到菜单栏) | $47                                                          | [安装包备份](https://github.com/insv23/MacOS/blob/main/installers/SoundSource%205.6.0_MacApp.dmg) |                                                              |
| [Hammerspoon](https://www.hammerspoon.org/)                  | 功能强大的脚本自动化工具，如[窗口管理](https://github.com/insv23/dotfiles/tree/main/hammerspoon) | 免费                                                         | hammerspoon                                                  |                                                              |
| [Bartender](https://www.macbartender.com/)                   | 隐藏菜单栏图标                                               | $16                                                          | [安装包备份](https://github.com/insv23/MacOS/tree/main/installers/Bartender%204.2.22) | [Hidden Bar](https://github.com/dwarvesf/hidden)             |
| [MacStroke](https://github.com/mtjo/MacStroke/blob/master/README_en.md) | 鼠标手势                                                     | 免费                                                         | macstroke                                                    |                                                              |
| [Mac Mouse Fix](https://mousefix.org/)                       | 鼠标平滑滚动，中间侧键自定义                                 | 免费                                                         | mouse-fix                                                    |                                                              |
| [KeyboardHolder](https://keyboardholder.leavesc.com/)        | 设置程序默认输入法                                           | 免费                                                         | keyboardholder                                               |                                                              |
| [NTFSTool](https://ntfstool.com/)                            | 免费的 NTFS 读写工具                                         | 免费                                                         | ntfstool                                                     |                                                              |
| [Bitwarden](https://bitwarden.com/)                          | 密码管理                                                     | 免费(自建)                                                   | bitwarden                                                    |                                                              |
| [AltTab](https://alt-tab-macos.netlify.app/)                 | 模仿 win 平台 alt tab 切换软件时显示窗口                     | 免费                                                         | alt-tab                                                      |                                                              |
| [Amphetamine](https://apps.apple.com/us/app/amphetamine/id937984704?mt=12) | 让 mac 不休眠                                                | 免费                                                         |                                                              | [Caffeinated](https://caffeinated.app/) [Coffee Buzz](https://coffeebuzz.aaronpantling.com/appstore-redirect/) |
| [OrbStack](https://orbstack.dev/)                            | 比 Docker Desktop 启动速度快、网络快、Rosetta x86 模拟、低 CPU 占用、低电量消耗。<br />替代 Linux 虚拟机。[介绍](https://www.appinn.com/orbstack/) | 免费(测试阶段)                                               | orbstack                                                     |                                                              |
| [iina](https://iina.io/)                                     | 播放器                                                       | 免费                                                         | iina                                                         |                                                              |
| [Keysmith](https://www.keysmith.app/)                        | 录制并重现你的操作                                           | 免费可设置五个动作                                           | keysmith                                                     |                                                              |
| [Syncthing](https://syncthing.net/)                          | P2P 多台设备之间文件同步 [使用 Syncthing 同步安卓手机和电脑文件](https://blog.insv.xyz/syncthing) | 免费                                                         | syncthing                                                    |                                                              |
| [MenubarX](https://menubarx.app/)                            | 菜单栏浏览器 在菜单栏打开任意网页                            | ¥ 29 买断(已购)                                              | menubarx                                                     |                                                              |
| 微信                                                         |                                                              |                                                              | wechat                                                       |                                                              |
| Telegram Desktop                                             |                                                              |                                                              | telegram-desktop                                             |                                                              |
| QQ                                                           |                                                              |                                                              | qq                                                           |                                                              |
| 腾讯会议                                                     |                                                              |                                                              | tencent-meeting                                              |                                                              |
| 百度网盘                                                     |                                                              |                                                              | baidunetdisk                                                 |                                                              |
| [小白羊云盘](https://github.com/gaozhangmin/aliyunpan)       | 第三方阿里网盘客户端                                         | 免费                                                         |                                                              |                                                              |
| QQ 音乐                                                      |                                                              |                                                              | qqmusic                                                      |                                                              |
| Autodesk Fusion 360                                          | 建模软件                                                     | 订阅制                                                       | autodesk-fusion360                                           |                                                              |
| [Horo](https://apps.apple.com/us/app/horo-timer-for-menu-bar/id1437226581?mt=12) | 菜单栏倒计时                                                 | 免费，¥68 解锁[完全功能](https://matthewpalmer.net/horo-free-timer-mac/horo-pro.html) (未购) |                                                              | [Timer_RH安装包](https://github.com/insv23/MacOS/blob/main/installers/Timer_RH_2.11.2__iMacSO.com.dmg) |
| [CrossOver](https://www.codeweavers.com/crossover)           | 在 Mac 系统上运行 Windows 应用，不必重启系统，不必使用虚拟机。[视频介绍及优惠码](https://www.bilibili.com/video/BV1Q64y197w5/) | ¥ 128 [购买](https://www.crossoverchina.com/buy.html?utm_source=https%3A%2F%2Fsouurl.cn%2F&utm_campaign=lm_alex&wm_cs_key=d2284b6e-7494-4d24-9376-9d28b68dd525)22版永久授权 | crossover                                                    |                                                              |

​	
