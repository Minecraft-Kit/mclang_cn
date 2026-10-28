# 安装与使用

本文介绍基岩版中文译名修正包的安装方法。 **普通玩家推荐直接导入`.mcpack`文件**；只有在导入失败或有特殊需求时，才需要尝试手动安装。

安装前请从[**GitHub Releases**](https://github.com/Minecraft-Kit/mclang_cn/releases)下载与你的游戏版本对应的语言包。其他下载渠道见[**README**](README.md#-下载)。

## 一、直接导入`.mcpack`（推荐）

### Windows

双击下载的`.mcpack`文件，Minecraft通常会自动启动并导入资源包。如果安装了多个Minecraft版本，可以右键点击文件，选择 **打开方式**，再选择目标版本。

### Android与iOS

在系统文件管理器中找到`.mcpack`文件并打开。如果出现应用选择界面，选择Minecraft。部分文件管理器可能把它识别为压缩文件，此时可尝试使用 **打开方式**，并指定Minecraft。

### 激活资源包

1. 打开Minecraft，进入 **设置 -> 通用 -> 全局资源**。
2. 在 **我的资源包**中找到 **中文译名修正包**，选择 **激活**。
3. 将其移动到 **已激活资源包**列表的最顶端。

语言包的位置决定其优先级。如果其他资源包包含相同翻译键，位于更高优先级的资源包可能覆盖本项目的文本。

> 语言包适配范围以对应版本的发布说明为准。不同平台和游戏版本的设置名称可能略有不同。

## 二、手动安装资源包

如果`.mcpack`无法自动导入，可以将它解压后放入游戏的`resource_packs`目录。

### 1. 解压语言包

`.mcpack`本质上是资源包文件，可使用支持ZIP格式的压缩工具打开；必要时也可将扩展名改为`.zip`后解压。

请保留资源包的顶层文件夹。文件结构应类似：

```text
CTR_xxx_xxx/
├── texts/
│   └── zh_CN.lang
├── manifest.json
└── ...
```

### 2. 复制到资源包目录

以下路径是参考示例，实际位置可能因游戏版本、安装方式、存储设备和系统权限而有所不同。

**Windows**

| 版本      | 资源包目录示例                                                                                                                      |
|:----------|:------------------------------------------------------------------------------------------------------------------------------------|
| UWP正式版 | `C:\Users\[用户名]\AppData\Local\Packages\Microsoft.MinecraftUWP_8wekyb3d8bbwe\LocalState\games\com.mojang\resource_packs\`         |
| UWP预览版 | `C:\Users\[用户名]\AppData\Local\Packages\Microsoft.MinecraftWindowsBeta_8wekyb3d8bbwe\LocalState\games\com.mojang\resource_packs\` |
| GDK正式版 | `C:\Users\[用户名]\AppData\Roaming\Minecraft Bedrock\Users\Shared\games\com.mojang\resource_packs\`                                 |
| GDK预览版 | `C:\Users\[用户名]\AppData\Roaming\Minecraft Bedrock Preview\Users\Shared\games\com.mojang\resource_packs\`                         |

如果使用其他磁盘安装旧版UWP应用，路径也可能位于对应磁盘的`WpSystem`目录中。不要仅依据游戏程序的安装盘符猜测资源包目录。

**Android**

| 存储路径                     | 资源包目录示例                                                                       |
|:-----------------------------|:-------------------------------------------------------------------------------------|
| 内部存储路径 | `/data/user/0/com.mojang.minecraftpe/games/com.mojang/resource_packs/`               |
| 外部存储路径                 | `/sdcard/Android/data/com.mojang.minecraftpe/files/games/com.mojang/resource_packs/` |

部分修改版安装包可能使用不同的包名，例如`com.mojang.minecraftbe`；此时需要按照实际包名调整路径。Android新版系统可能限制访问`Android/data`，而`/data/user/0`通常也无法由普通文件管理器直接访问。

**iOS**

由于iOS应用沙盒限制，一般不建议通过手动复制方式安装。优先使用上一节介绍的`.mcpack`导入方法。

### 3. 检查文件结构并激活

复制完成后，确认`resource_packs`下存在资源包文件夹，且文件夹内部直接包含`manifest.json`，不要多套一层目录。

```text
.../
└── resource_packs/
    ├── CTR_xxx_xxx/
    │   ├── texts/
    │   │   └── zh_CN.lang
    │   ├── manifest.json
    │   └── ...
    └── ...
```

然后重新启动游戏，并按照第一节的步骤在 **全局资源**中激活语言包。

## 三、直接修改游戏语言文件（高级用户）

> **此方法不推荐普通玩家使用。** 它会修改游戏安装文件，可能受到系统权限和签名校验限制，也可能在游戏更新后失效。请先备份原始文件，确认自己有权修改相关安装文件，并优先考虑前两种资源包安装方式。

某些游戏版本的翻译分散在多个语言文件中，直接替换某个`zh_CN.lang`不一定能够覆盖所有文本。 **不能只凭文件名批量删除或覆盖其他语言文件。**

### Windows

Windows上的游戏资源文件位置与安装程序版本（UWP、GDK）有关：

| 版本      | 安装数据目录示例                                                                                   |
|:----------|:---------------------------------------------------------------------------------------------------|
| UWP正式版 | `C:\Program Files\WindowsApps\Microsoft.MinecraftUWP_[版本号]_[架构]__8wekyb3d8bbwe\data\`         |
| UWP预览版 | `C:\Program Files\WindowsApps\Microsoft.MinecraftWindowsBeta_[版本号]_[架构]__8wekyb3d8bbwe\data\` |
| GDK正式版 | `C:\XboxGames\Minecraft for Windows\Content\data\`                                                 |
| GDK预览版 | `C:\XboxGames\Minecraft Preview for Windows\Content\data\`                                         |

如需修改语言文件，先确认正确的数据目录与实际使用的语言文件，备份后再针对对应版本进行修改。`WindowsApps`等目录通常受系统保护，不建议为修改翻译而随意更改系统目录权限。

### Android

Android游戏资源通常位于安装包的`assets/assets`目录下，部分版本的语言文件还可能拆分到多个资源包中。

直接修改需要处理安装包内容，并可能涉及重新打包、签名及安装；具体方法因APK、拆分安装包及设备环境而异。请先核实实际文件来源与使用方式，避免覆盖其他平台或版本专用的语言文件。

### iOS

iOS游戏资源通常位于应用安装包内部，例如`Payload/minecraftpe.app/data`。修改IPA可能受到应用签名、系统权限和安装方式的限制；普通用户应优先使用`.mcpack`导入。

### 关于重复翻译键

项目语言文件可能汇集多个英文源文件的翻译，部分条目为平台或版本差异而保留，个别重复翻译键还可能被注释。

直接替换游戏原始语言文件时，应根据目标版本的文件结构检查翻译键及加载顺序。 **注释掉的译文不会自动根据平台启用；也不要在没有核实来源和行为的情况下删除或解除注释。**

另一种高级用法是将项目译文按来源分段合并到游戏对应的语言文件，但需要逐段核对翻译键、重复定义及加载方式。

## 四、主机平台说明

Xbox、PlayStation和Nintendo Switch通常不提供与Windows或移动端相同的`.mcpack`直接导入方式。

某些世界可以通过Realms或其他受支持的方式共享世界资源包，但 **这不等于在主机上安装全局语言包**，也不能保证修改主菜单等全局界面文本。是否能够应用本项目的翻译，取决于平台及游戏版本的资源包加载限制。

## 五、常见问题

**导入成功，但没有看到译文变化？** 检查语言包是否在 **全局资源**中激活、是否放在列表顶部，以及下载版本是否与你的游戏版本匹配。

**Minecraft无法识别`.mcpack`？** 检查下载文件是否完整；尝试使用系统的 **打开方式**选择Minecraft，或按第二节手动安装。

**更新游戏后语言包失效？** 查看项目的[**最新发布说明**](https://github.com/Minecraft-Kit/mclang_cn/releases)，确认是否已有适配版本。直接替换游戏文件的方式通常需要重新处理。

遇到其他问题，可以前往[**GitHub Issues**](https://github.com/Minecraft-Kit/mclang_cn/issues)反馈，并注明游戏版本、平台、安装方式及具体表现。
