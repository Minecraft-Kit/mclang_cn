<div align="center">

   <img src="Minecraft.png" alt="Minecraft" width="400px">

# 基岩版中文译名修正

### 让基岩版也可以拥有更好的中文

#### 修正官方译文 · 统一游戏术语 · 补全版本内容

   <img src="KeyArt.jpg" alt="KeyArt" width="400px">

#### [![星标数](https://img.shields.io/github/stars/Minecraft-Kit/mclang_cn?color=eac54f&style=for-the-badge&label=星标数)](https://github.com/Minecraft-Kit/mclang_cn/stargazers) [![总下载](https://img.shields.io/github/downloads/Minecraft-Kit/mclang_cn/total?style=for-the-badge&label=总下载)](https://github.com/Minecraft-Kit/mclang_cn/releases) [![仓库大小](https://img.shields.io/github/repo-size/Minecraft-Kit/mclang_cn?style=for-the-badge&label=仓库大小)](https://github.com/Minecraft-Kit/mclang_cn/archive/refs/heads/main.zip)

#### [![最近提交](https://img.shields.io/github/last-commit/Minecraft-Kit/mclang_cn?style=for-the-badge&label=最近提交)](https://github.com/Minecraft-Kit/mclang_cn/commits/main) [![开源许可](https://img.shields.io/badge/开源许可-CC%20BY--NC--SA%204.0-ff69b4?style=for-the-badge)](LICENSE)

</div>

---

## 📖 关于项目

**基岩版中文译名修正**是一个以个人维护为主、开放社区贡献的 Minecraft 简体中文语言修正项目。

项目主要修正 Minecraft 基岩版既有简体中文中的**错译、漏译、语义偏差、术语不统一及格式问题**，并根据实际版本补充隐藏文本、调试信息，以及部分平台、版本和编辑器独有的语言内容。

项目优先考证已有译名：**中文 Minecraft Wiki → Minecraft Crowdin → 其他可信资料 → 明确标记的自主拟译**。当 Java 版与基岩版存在对应的同一内容、但名称不同的情况时，原则上**优先采用 Java 版简体中文译名**；具体仍需结合对象、版本及上下文核实。

### 🌐 [项目网站](https://kit.minecraft.spectrollay.com/mclang_cn/)

项目网站使用 [OreUI](https://github.com/Spectrollay-OreUI/OreUI) 技术构建。访问和使用项目网站，即代表你已阅读并同意相关使用条款与免责声明。

### 🎮 适用范围

本项目主要面向基于 **基岩引擎**开发的 Minecraft 游戏版本，包括：

* **基岩版 | 教育版 | 试玩版 | 基岩版编辑器**

不同平台及版本的具体使用方式可能有所不同，请参阅下方的 [安装使用](#-安装使用) 章节。

---

## ✨ 项目特点

| 特点            | 说明                                                     |
|:----------------|:---------------------------------------------------------|
| 🎯 **逐键校对** | 按翻译键对照原始英文，检查错译、漏译、键值及参数错误。 |
| 📖 **语义优化** | 保留原文的信息与语气，并尊重合理的项目既有表达。     |
| 🧩 **术语统一** | 参考 Minecraft Wiki、Java 版译名及上下文统一术语。   |
| 🔍 **内容补充** | 适配隐藏文本、调试信息以及部分平台或版本独有的内容。     |
| ⚡ **持续更新** | 持续跟进 Minecraft 正式版及开发版的语言内容变化。        |
| 📦 **开箱即用** | 以标准 `.mcpack` 资源包形式发布，导入后即可使用。        |
| 🤝 **社区驱动** | 欢迎提交问题、建议与贡献，共同完善项目。                 |

---

## 🧭 译名依据与校对规范

本项目不仅修正字面翻译，也重视**Java 版与基岩版的译名对应、游戏内上下文、格式完整性，以及同一术语在不同界面中的一致性**。译文与官方基岩版简体中文不同，并不一定代表错误。

| 核对环节 | 基本原则 |
|:--|:--|
| **译名考证** | 优先查阅[中文 Minecraft Wiki](https://zh.minecraft.wiki/)；同一内容有不同版本译名时，优先采用 Java 版简体中文。若没有可靠依据，再查 [Minecraft Crowdin](https://crowdin.com/translate/minecraft/10038/enus-zhcn)和其他资料。 |
| **语义与上下文** | 核对界面用途、前后文、跨 key 拼接句子，以及动态参数所代表的真实对象。 |
| **翻译键与文件** | 按 key 而非行号比较，不擅改 key；保留来源分段、注释、平台差异与项目定制文本。 |
| **格式与符号** | 保留占位符、按键标记、控制字符；句末标点双向对应，普通中文使用全角括号，保留技术文本的原始语法。 |
| **表达与风格** | 汉字与英文、数字之间默认不加空格；按键名称可使用中文双引号；尊重准确且合理的现有译法。 |

现有官方中文仅供对照，仓库自身的旧译文用于保持一致，**两者都不能替代独立的译名考证**。资料不足的译文应标记待审核，而不是未经确认就宣称采用了权威译名。

> **参与修订前，请阅读 [贡献指南（CONTRIBUTING.md）](CONTRIBUTING.md)。** 其中包含完整的来源优先级、占位符调序示例、标点与空格规范、重复 key 和分段文件处理规则。

### 📁 关于翻译文件

项目中的 `zh_CN.lang` 可能按分段整合多个英文原始语言文件。部分注释、历史内容与部分自定义文本为项目有意保留的内容；某个版本的英文原文未包含某个 key，不代表该中文条目一定无效。

另外，**Preview／Beta、不同平台、教育版及编辑器可能存在不同文本和重复 key**。维护时应先确认来源与实际使用环境，不能根据单份英文文件机械清理所有未匹配条目。

---

## 🚀 安装使用

### 1. 下载语言包

你可以从 GitHub、Gitee、Gitea 或项目官方网盘获取语言包。

![正式版](https://img.shields.io/github/v/release/Minecraft-Kit/mclang_cn?style=for-the-badge&label=正式版) ![发布于](https://img.shields.io/github/release-date/Minecraft-Kit/mclang_cn?style=for-the-badge&label=发布于)

> 适用于正式版的稳定更新。具体适配版本及更新内容请参阅对应的发布说明。

下载： [GitHub](https://github.com/Minecraft-Kit/mclang_cn/releases/latest) | [Gitee](https://gitee.com/Spectrollay/mclang_cn/releases) | [Gitea](https://gitea.com/Spectrollay/mclang_cn/releases/latest) | [项目官方网盘](https://pan.huang1111.cn/s/E74A7Fb)

![最新版](https://img.shields.io/github/v/release/Minecraft-Kit/mclang_cn?include_prereleases&style=for-the-badge&label=最新版) ![发布于](https://img.shields.io/github/release-date-pre/Minecraft-Kit/mclang_cn?style=for-the-badge&label=发布于)

> 包含正式版及预览版发布。预览版主要用于测试开发版适配以及语言包自身的更新，可能会不大稳定。

下载： [GitHub](https://github.com/Minecraft-Kit/mclang_cn/releases) | [Gitee](https://gitee.com/Spectrollay/mclang_cn/releases) | [Gitea](https://gitea.com/Spectrollay/mclang_cn/releases) | [项目官方网盘](https://pan.huang1111.cn/s/E74A7Fb)

---

### 2. 安装语言包

下载 `.mcpack` 文件后，可以根据你的使用场景选择以下方式。

#### (1) 直接导入 `.mcpack`（推荐）

这是最简单、最适合普通用户的安装方式。

##### ● Windows

直接 **双击 `.mcpack` 文件**，Minecraft 通常会自动导入资源包。

如果设备上同时安装了多个 Minecraft 版本，可以：

1. 右键点击 `.mcpack` 文件；
2. 选择 **打开方式**；
3. 选择希望导入的 Minecraft 版本。

##### ● Android / iOS

使用系统文件管理器找到 `.mcpack` 文件并点击。

如果系统询问打开方式，请选择 Minecraft。

部分文件管理器可能会将 `.mcpack` 识别为文本文件或压缩文件，此时可以通过 **打开方式**手动选择 Minecraft。

> 如果设备上安装了多个 Minecraft 版本，请注意选择正确的版本。

##### ● Xbox / PlayStation / Nintendo Switch

主机平台通常无法直接导入 `.mcpack` 文件。

一种常见方式是：

1. 在 Windows 或移动设备上导入语言包；
2. 创建或打开一个世界；
3. 通过 **Minecraft Realms** 同步带有资源包的世界；
4. 在主机端进入该世界。

也可以使用第三方存档编辑工具进行处理，但相关操作可能较为复杂，并存在数据损坏风险，请自行做好备份。

#### (2) 手动复制资源包

如果 `.mcpack` 无法正常导入，或者你希望直接管理资源包文件，可以使用此方法。

##### ① 解压语言包

将 `.mcpack` 文件重命名为 `.zip`，例如：

```text
CTR_xxx_xxx.mcpack
↓
CTR_xxx_xxx.zip
```

然后解压文件。

解压后请 **保留最外层的语言包文件夹**，目录结构通常类似：

```text
CTR_xxx_xxx/
├── texts/
│   └── zh_CN.lang
├── manifest.json
└── ...
```

其中 `CTR_xxx_xxx/` 是语言包的顶层文件夹。

##### ② 将语言包复制到 `resource_packs`

根据你的平台，将整个 `CTR_xxx_xxx/` 文件夹复制到对应的 `resource_packs` 目录。

##### ● Windows

| 版本       | 默认路径                                                                                                                           | 自定义 D 盘安装路径                                                                                                                       |
|:-----------|:-----------------------------------------------------------------------------------------------------------------------------------|:------------------------------------------------------------------------------------------------------------------------------------------|
| UWP 正式版 | `C:\Users\[用户名]\AppData\Local\Packages\Microsoft.MinecraftUWP_8wekyb3d8bbwe\LocalState\games\com.mojang\resource_packs`         | `D:\WpSystem\[设备标识符]\AppData\Local\Packages\Microsoft.MinecraftUWP_8wekyb3d8bbwe\LocalState\games\com.mojang\resource_packs`         |
| UWP 开发版 | `C:\Users\[用户名]\AppData\Local\Packages\Microsoft.MinecraftWindowsBeta_8wekyb3d8bbwe\LocalState\games\com.mojang\resource_packs` | `D:\WpSystem\[设备标识符]\AppData\Local\Packages\Microsoft.MinecraftWindowsBeta_8wekyb3d8bbwe\LocalState\games\com.mojang\resource_packs` |
| GDK 正式版 | `C:\Users\[用户名]\AppData\Roaming\Minecraft Bedrock\Users\Shared\games\com.mojang\resource_packs`                                 | 同默认安装目录                                                                                                                            |
| GDK 开发版 | `C:\Users\[用户名]\AppData\Roaming\Minecraft Bedrock Preview\Users\Shared\games\com.mojang\resource_packs`                         | 同默认安装目录                                                                                                                            |

##### ● Android

| 版本   | 内部存储路径                                                          | 外部存储路径                                                                        |
|:-------|:----------------------------------------------------------------------|:------------------------------------------------------------------------------------|
| 标准版 | `/data/user/0/com.mojang.minecraftpe/games/com.mojang/resource_packs` | `/sdcard/Android/data/com.mojang.minecraftpe/files/games/com.mojang/resource_packs` |
| 改包版 | `/data/user/0/com.mojang.minecraftbe/games/com.mojang/resource_packs` | `/sdcard/Android/data/com.mojang.minecraftbe/files/games/com.mojang/resource_packs` |

> Android 版本、设备权限及文件管理器可能影响实际路径和访问方式。本处假设改包版包名为 `com.mojang.minecraftbe`。

##### ● iOS

由于 iOS 的应用沙盒机制，普通用户通常无法直接访问 Minecraft 的内部文件。

因此， **iOS 用户建议优先使用方法一导入 `.mcpack`，或者通过 Minecraft Realms 同步资源包。**

手动修改游戏文件通常需要越狱设备或其他特殊工具，并可能带来数据丢失、应用异常等风险。

##### ③ 确认目录结构

复制完成后，目录结构应类似：

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

#### (3) 直接替换游戏语言文件（高级用户）

> ⚠️ **高级操作**
>
> 此方法会直接修改 Minecraft 的安装文件。
>
> 操作不当可能导致游戏无法启动、更新失败或数据损坏。
> **开始操作前请务必备份原始文件。**

该方法适合熟悉 Minecraft 文件结构、APK/IPA 或 Windows 应用文件的高级用户。不同版本的资源文件位置和加载方式可能不同，**请优先使用资源包导入，不建议仅凭文件名批量删除或覆盖安装目录**。

##### ● Windows

首先从语言包中提取 `zh_CN.lang`，然后定位 Minecraft 的安装数据目录。

| 版本                | 默认路径                                                                                          | 自定义 D 盘安装路径                                                                 |
|:--------------------|:--------------------------------------------------------------------------------------------------|:------------------------------------------------------------------------------------|
| UWP 正式版          | `C:\Program Files\WindowsApps\Microsoft.MinecraftUWP_[版本号]_[架构]__8wekyb3d8bbwe\data`         | `D:\WindowsApps\Microsoft.MinecraftUWP_[版本号]_[架构]__8wekyb3d8bbwe\data`         |
| UWP 测试版 / 预览版 | `C:\Program Files\WindowsApps\Microsoft.MinecraftWindowsBeta_[版本号]_[架构]__8wekyb3d8bbwe\data` | `D:\WindowsApps\Microsoft.MinecraftWindowsBeta_[版本号]_[架构]__8wekyb3d8bbwe\data` |
| GDK 正式版          | `C:\XboxGames\Minecraft for Windows\Content\data`                                                 | `D:\XboxGames\Minecraft for Windows\Content\data`                                   |
| GDK 预览版          | `C:\XboxGames\Minecraft Preview for Windows\Content\data`                                         | `D:\XboxGames\Minecraft Preview for Windows\Content\data`                           |

> 由于 `WindowsApps` 和 `XboxGames` 目录受到系统权限保护，你可能需要管理员权限才能访问。

在数据目录及其子目录中：

1. 搜索所有 `zh_CN.lang` 文件；
2. 备份原始文件；
3. 核实需要替换的实际语言文件位置，不要一次性删除所有同名文件；
4. 找到与目标版本对应的 `resource_packs\vanilla\texts`；
5. 在确认备份可恢复后，替换目标目录中的 `zh_CN.lang`。

最终结构类似：

```text
data/
├── resource_packs/
│   ├── vanilla/
│   │   ├── texts/
│   │   │   ├── en_US.lang
│   │   │   ├── zh_CN.lang
│   │   │   └── ...
│   │   └── ...
│   └── ...
└── ...
```

完成后重新启动游戏即可。

##### ● Android

首先，获取 Minecraft 安装包，通常为 `.apk` 或 `.apks`。
如果获取到的是 `.apks`，需使用兼容该格式的工具处理；拆包、重新签名或修改安装包可能受到平台安全机制及正版校验的限制。请仅操作你有权修改的安装文件。

然后：

1. 使用解压或 APK 工具打开安装包；
2. 定位到 `/assets/assets`；
3. 查找目标版本中的 `zh_CN.lang`，并识别其对应的平台或分段；
4. 备份原始文件；
5. 不要未经核实就删除其他目录里的同名语言文件；
6. 定位到 `/resource_packs/vanilla/texts`；
7. 将项目提供的 `zh_CN.lang` 放入正确位置，确认其覆盖关系；
8. 重新打包并签名 APK；
9. 安装修改后的游戏。

> **关于重复键**
>
> 由于 Android 版本的语言文件可能被拆分为多个文件，直接替换后可能存在键值重复的问题。
> 本项目提供的语言文件中，对于重复键通常仅保留适用范围最广的一条，其余内容会被注释。如果需要使用其他译文，可以根据实际情况手动解除注释。

当然，另一种方式是不删除原有语言文件，而是将项目提供的译文按照章节分别复制到对应的 `zh_CN.lang` 文件中。

这种方式可以更加精确地保留游戏原有的文件结构，但需要逐个处理所有相关语言文件，操作也更加繁琐。

##### ● iOS

首先获取 Minecraft 的 `.ipa` 安装包。

然后：

1. 解压 `.ipa`；
2. 定位到 `/Payload/minecraftpe.app/data`；
3. 查找目标版本中的 `zh_CN.lang`，并识别其对应的平台或分段；
4. 备份原始文件；
5. 不要未经核实就删除其他目录里的同名语言文件；
6. 定位到 `/resource_packs/vanilla/texts`；
7. 将项目提供的 `zh_CN.lang` 放入正确位置，确认其覆盖关系；
8. 重新打包 `.ipa`；
9. 根据设备环境完成重新签名及安装。

与 Android 类似，部分 iOS 版本的语言文件可能存在拆分及重复键问题。

如果不希望删除原文件，也可以按照章节将项目提供的译文分别复制到对应的 `zh_CN.lang` 中。

> iOS 对未签名或重新签名的 `.ipa` 安装存在额外限制，具体操作取决于设备环境及所使用的安装工具。

### 3. 激活语言包

如果你使用的是 **方法一或方法二**，完成导入后还需要在 Minecraft 中启用语言包。

1. 打开 Minecraft，在主界面进入 **设置**；
2. 在侧边栏的 **通用** 中找到 **全局资源**；
3. 在 **我的资源包** 中找到 **中文译名修正包**；
4. 点击资源包，并选择 **激活**；
5. 确认语言包位于 **已激活资源包** 列表的最顶端。

如果语言包没有位于最顶端，可以选中语言包后，使用下方的 **向上箭头**将其移动到最顶部。

> **为什么需要放在最顶端？**
>
> Minecraft 的资源包会按照优先级处理相同资源。将本项目放在最顶端，可以确保修正后的语言文件优先于其他资源包中的对应文件。

---

## 🤝 参与贡献

这是一个持续维护的社区项目，我们欢迎任何形式的贡献。

你可以通过以下方式参与：

* 提交翻译问题；
* 提出术语修改建议；
* 报告遗漏或错误；
* 提交新的文本修正；
* 协助适配新的 Minecraft 版本。

完整的译名来源优先级、翻译格式规范及提交要求，请参阅 **[贡献指南](CONTRIBUTING.md)**。

---

## 💬 联系与交流

如果你希望反馈问题、讨论翻译或获取使用帮助，可以加入我们的社区：

[![Telegram](https://img.shields.io/badge/Telegram-群组-blue?style=for-the-badge)](https://t.me/spectrollay_workshop) [![QQ](https://img.shields.io/badge/QQ-群组-blue?style=for-the-badge)](https://qm.qq.com/q/AqLmKLH9mM) [![云湖](https://img.shields.io/badge/云湖-群组（已弃用）-blue?style=for-the-badge)](https://yhfx.jwznb.com/share?key=VyTE7W7sLwRl&ts=1684642802)

---

## 🔗 相关链接

### 项目

* **本项目隶属于**: [Minecraft 工具包](https://github.com/Minecraft-Kit)
* **项目网站：** [基岩版中文译名修正](https://kit.minecraft.spectrollay.com/mclang_cn/)
* **源代码：** [GitHub](https://github.com/Minecraft-Kit/mclang_cn)

### 参考资料

* [Minecraft Wiki](https://zh.minecraft.wiki)
* [Crowdin](https://crowdin.com/translate/minecraft/10038/enus-zhcn)

---

## 📜 开源许可

本项目基于 **[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International (CC BY-NC-SA 4.0)](LICENSE)** 许可协议授权。

在遵守许可协议的前提下，你可以：

* **共享** — 以任何媒介或格式复制、发行本作品；
* **演绎** — 修改、转换本作品，或基于本作品进行创作。

但必须遵守以下条件：

* **署名（BY）** — 必须给予适当署名，并提供许可证链接，同时说明是否进行了修改；
* **非商业性（NC）** — 不得将本作品用于商业目的；
* **相同方式共享（SA）** — 如果基于本作品进行再创作，必须以相同许可协议发布。

完整许可条款请参阅 [LICENSE](LICENSE)。

---

<div align="center">

**© 2020 Spectrollay | 用❤️制作**

<sub>本项目与 Mojang Studios、Microsoft 或 Minecraft 官方没有隶属关系。</sub>

</div>
