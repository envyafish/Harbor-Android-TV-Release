<div align="center">

<img src="docs/logo.png" width="120" height="120" alt="Harbor TV">

# Harbor TV（港湾电视版）

**面向 [Emby](https://emby.media/) / [Jellyfin](https://jellyfin.org/) 的桌面与电视客户端**

[![电视版](https://img.shields.io/github/v/release/envyafish/Harbor-Android-TV-Release?style=flat-square&label=tv)](https://github.com/envyafish/Harbor-Android-TV-Release/releases/latest)
[![桌面版](https://img.shields.io/github/v/release/envyafish/Harbor?style=flat-square&label=desktop)](https://github.com/envyafish/Harbor/releases/latest)
[![Downloads](https://img.shields.io/github/downloads/envyafish/Harbor-Android-TV-Release/total?style=flat-square)](https://github.com/envyafish/Harbor-Android-TV-Release/releases)

[下载](https://github.com/envyafish/Harbor-Android-TV-Release/releases/latest) · [桌面端 Harbor](https://github.com/envyafish/Harbor) · [反馈 Bug](https://github.com/envyafish/Harbor-Android-TV-Release/issues) · [购买](https://pay.ldxp.cn/shop/767OK1ZS) · [TG 交流群](https://t.me/HarborRelease)

</div>

---

Harbor 有两个产品：

- **[Harbor 桌面端](https://github.com/envyafish/Harbor)** — macOS / Windows，内嵌 **libmpv** 播放，适合日常浏览、续看、统计与弹幕
- **Harbor TV** — Android TV / Google TV，为客厅遥控重新设计

亦兼容 [极影视](https://www.zspace.cn/)（桌面端，缺乏充分测试）。

---

## 购买

可通过 [店铺](https://pay.ldxp.cn/shop/767OK1ZS) 购买 Harbor Pro。同一许可证可用于桌面端与 Harbor TV。

<img src="docs/shop.png" alt="店铺二维码" width="220" />

---

## Harbor 桌面端

桌面端面向 Emby / Jellyfin 的日常使用：侧栏切换媒体库，首页继续观看，详情页选音轨与字幕，再用内嵌 libmpv 播放。账号与令牌保存在系统钥匙串，不需要 Harbor 云账号。

完整安装包见 [Harbor](https://github.com/envyafish/Harbor)。

### 首页

打开后是 Hero 推荐与媒体库入口。下方是继续观看，以及各库的最新内容；剧集海报会标出未看集数。

<img src="docs/screenshots/pc/home-hero.png" alt="首页 Hero 与媒体库" width="100%" />

<img src="docs/screenshots/pc/home-continue.png" alt="继续观看与最新内容" width="100%" />

### 媒体库

每个库是海报网格。可按全部 / 继续观看 / 未观看 / 已观看 / 收藏筛选，也可按年份、评分、添加日期排序，并搜索本库。

<img src="docs/screenshots/pc/library.png" alt="媒体库网格" width="100%" />

### 详情

电影与剧集都是沉浸式详情：海报取色背景、播放 / 收藏 / 已看、音轨与字幕、媒体信息，以及 IMDb、TMDb、Trakt 外链。剧集页可按季浏览，点进单集继续看。

详情页还可以**生成本地中文字幕**（Pro）：从音轨识别，日语可直译或转译。

<img src="docs/screenshots/pc/detail-movie.png" alt="电影详情" width="100%" />

<img src="docs/screenshots/pc/detail-series.png" alt="剧集详情" width="100%" />

向下滚动可见章节、演职员与相似内容。点演员会进入作品列表。

<img src="docs/screenshots/pc/detail-cast.png" alt="章节、演职员与相似内容" width="100%" />

<img src="docs/screenshots/pc/detail-episodes.png" alt="剧集分集列表" width="100%" />

<img src="docs/screenshots/pc/people.png" alt="演职员页" width="100%" />

### 收藏与搜索

收藏按媒体库分组。搜索支持电影、剧集、单集、音乐与演职员，并记住最近关键词。

<img src="docs/screenshots/pc/favorites.png" alt="收藏" width="100%" />

<img src="docs/screenshots/pc/search.png" alt="搜索" width="100%" />

### 播放器

内嵌 libmpv，Direct Play / Direct Stream 自动回退。进度条、倍速、音量、音轨 / 字幕 / 双字幕、弹幕、画中画、全屏都在播放器里完成。进度会回写服务器。

<img src="docs/screenshots/pc/player.png" alt="桌面播放器" width="100%" />

播放相关能力：

- **原生播放** — macOS / Windows 随应用分发 libmpv；也可改用外部 mpv / VLC / PotPlayer，并同步进度
- **字幕** — 服务器字幕轨、本地外挂、双字幕；字号、位置、颜色、描边、底框可调
- **生成中文字幕（Pro）** — 本机 Whisper 识别音轨，可选译成中文，并可上传回 Emby
- **弹幕（Pro，可选）** — 兼容 danmu_api 的多源、热力条跳转、播放中换源；只看不发
- **Anime4K（Pro）** — 动画超分，可仅对动画生效
- **跳过片头片尾（Pro）** — 手动 / 自动延迟 / 自动即时；服务器无标记时用 IntroDB 补缺
- **HDR / 杜比** — 检测到 HDR10 / HDR10+ / HLG / 杜比视界时，可自动切独立窗口或外部播放器

### 观影统计

按月看总时长、电影 / 剧集占比、题材与年代，以及本月 Top 剧集 / 电影。还有星期偏好、时段分布、评分画像和连续打卡日历。

<img src="docs/screenshots/pc/stats.png" alt="观影统计总览" width="100%" />

<img src="docs/screenshots/pc/stats-top.png" alt="本月 Top 剧集与电影" width="100%" />

<img src="docs/screenshots/pc/stats-hours.png" alt="星期偏好与时段分布" width="100%" />

<img src="docs/screenshots/pc/stats-calendar.png" alt="连续打卡日历" width="100%" />

### 日历

连接 Trakt 后，按「播出 / 新剧」看本周或本月更新，方便追更。想看列表也在侧栏。

<img src="docs/screenshots/pc/calendar.png" alt="播出日历" width="100%" />

### 控制台

查看服务器上正在播放的会话、在线设备，必要时可踢出。播放历史可按今天 / 7 天 / 30 天筛选。

<img src="docs/screenshots/pc/console.png" alt="控制台在线设备" width="100%" />

<img src="docs/screenshots/pc/console-history.png" alt="控制台播放历史" width="100%" />

### 设置

设置按账号、媒体库、外观、播放、字幕、Trakt、弹幕、快捷键、存储、关于分区。播放页可调内置 / 外部播放器、默认音轨字幕语言、硬件解码、缓存、跳过片头片尾、字幕外观、Anime4K，以及生成本地字幕的识别模型。

<img src="docs/screenshots/pc/settings-playback.png" alt="播放设置" width="100%" />

<img src="docs/screenshots/pc/settings-subtitles.png" alt="字幕外观设置" width="100%" />

<img src="docs/screenshots/pc/settings-anime4k.png" alt="Anime4K 与生成字幕" width="100%" />

主题支持浅色 / 深色 / 跟随系统，多种强调色与背景。macOS 使用 Overlay 标题栏，Windows 为无边框自定义标题栏。

### 桌面端功能一览

- **媒体库** — 浏览视图、文件夹、剧集、电影、合集、播放列表
- **继续观看 / Next Up** — 断点续播；可从继续观看中移除
- **收藏、搜索、想看** — 侧栏直达
- **原生播放** — 内嵌 libmpv；可选外部播放器
- **字幕** — 服务器轨、本地外挂、双字幕、外观微调、本地生成中文字幕
- **弹幕** — 多源、热力条、播放中选源
- **Trakt** — 播放同步、已看对账、日历、想看
- **观影统计** — 月度时长、题材、打卡、Top 榜
- **控制台** — 在线会话与播放历史
- **安全会话** — 服务器账号与令牌保存在系统钥匙串

---

## Harbor TV

客厅版 Harbor，运行在 **Android TV / Google TV**。全屏沉浸、方向键操作，浏览与播放习惯与桌面端对齐，但按遥控重新做了交互。

需要 Harbor Pro 激活后使用。可用遥控器粘贴许可证，也可扫局域网二维码在手机 / 电脑上提交。

### 首页

满屏 Backdrop + 顶部横行挑片。有继续观看时，Hero 合并续看与 Next Up；焦点移动时背景、标题和「播放」按钮一起切换。往下是媒体库卡片，以及各库最新。

顶栏为 **首页 · 收藏 · 搜索**，右侧是账号、儿童模式与设置。

<img src="docs/screenshots/home.png" alt="Harbor TV 首页" width="100%" />

<img src="docs/screenshots/home-libraries.png" alt="Harbor TV 媒体库行" width="100%" />

### 媒体库

海报网格，可用全部 / 未看 / 已看 / 收藏 / 合集筛选，并按年份、类型、标题等排序。每个库会记住上次的筛选与排序。

<img src="docs/screenshots/library.png" alt="Harbor TV 媒体库网格" width="100%" />

### 详情

全宽背景、分辨率 / 时长 / 音轨信息，「继续」或从头播放，以及收藏、加入播放列表。音轨与字幕可在详情页选好再播。下方是演职员与相似影片。

<img src="docs/screenshots/detail.png" alt="Harbor TV 电影详情" width="100%" />

<img src="docs/screenshots/detail-similar.png" alt="Harbor TV 演职员与相似" width="100%" />

<img src="docs/screenshots/people.png" alt="Harbor TV 演职员页" width="100%" />

### 收藏与搜索

收藏按库分组。搜索页在未输入时展示服务器推荐，输入片名或剧名后自动出结果。

<img src="docs/screenshots/favorites.png" alt="Harbor TV 收藏" width="100%" />

<img src="docs/screenshots/search.png" alt="Harbor TV 搜索" width="100%" />

### 播放器

优先 Direct Play 原文件，不烧字幕。隐藏 OSD 时左右键 ±10 秒，并显示进度预览；上下键滑出完整控制条。剧集可在播放中选集，片尾约 8 秒倒计时下一集。

<img src="docs/screenshots/player.png" alt="Harbor TV 播放" width="100%" />

<img src="docs/screenshots/player-osd.png" alt="Harbor TV 播放器 OSD" width="100%" />

电视播放相关能力：

- **直出优先** — Direct Play；HDMI 音频透传，不能透传时本机软解
- **字幕** — 文本轨叠层；ASS/SSA 由本机 libass 渲染；支持双字幕
- **杜比视界 / HDR** — 本机映射与 SDR 屏 tone map；可匹配电视刷新率
- **跳过片头片尾** — 与桌面相同的四档；服务器无标记时用 IntroDB 补缺
- **弹幕** — 只看不发；OSD 开关与换源；可按媒体库关闭
- **暂停静帧** — 暂停一段时间后显示时钟，减少烧屏
- **系统续看** — 写入 Android TV Watch Next，可从系统主页接着播

### 儿童模式

指定一个账号并设置 4 位 PIN。可分别限制工作日 / 周末每日时长，以及最早 / 最晚开播。家长可用 PIN 查看看片记录。儿童模式下没有设置、换号和弹幕入口。

<img src="docs/screenshots/kids.png" alt="Harbor TV 儿童模式设置" width="100%" />

<img src="docs/screenshots/watch-log.png" alt="Harbor TV 看片记录" width="100%" />

### 电视端功能一览

- **客厅交互** — 无常驻侧栏，方向键移焦点；卡片长按可播放、标记已看、加入播放列表
- **多账号** — 局域网扫描或手动填地址；可用二维码在手机上完成登录
- **收藏 / 搜索** — 顶栏直达；搜索页带服务器推荐
- **播放** — Direct Play、双字幕、弹幕、跳过片头片尾、下一集倒计时
- **儿童模式** — PIN、每日时长、可看时段、看片记录
- **Trakt** — 设备码连接，同步播放进度
- **外观** — 与桌面一致的 16 种主题色；浏览页深色 / 浅色

---

## 支持平台

| 产品 | 平台 | 说明 |
|------|------|------|
| Harbor 桌面端 | macOS 26+（Apple Silicon / Intel） | Overlay 标题栏；原生播放随应用分发 |
| Harbor 桌面端 | Windows 10+（x64） | 无边框窗口；原生播放随应用分发 |
| Harbor TV | Android TV / Google TV（Android 7+） | 遥控 / 方向键；需 Harbor Pro |

当前桌面安装程序支持 **Windows 10**（x64）与 **macOS 26** 及以上。请把 Harbor TV 安装到 **电视机或电视盒子**，不要当作手机 / 平板应用使用。

---

## 支持的媒体服务器

| 服务器 | 桌面端 | Harbor TV |
|--------|--------|-----------|
| [Emby](https://emby.media/) | 主要支持 | 主要支持 |
| [Jellyfin](https://jellyfin.org/) | 已支持 | 已支持 |
| [极影视](https://www.zspace.cn/) | 兼容，缺乏充分测试 | 不支持 |

---

## 开始使用

**Harbor TV**

1. 从 [Releases](https://github.com/envyafish/Harbor-Android-TV-Release/releases) 下载最新 APK，用电视的「从 U 盘安装」或 `adb install` 装上。
2. 用 Harbor Pro 许可证激活（可用遥控器粘贴，或扫码在手机 / 电脑上提交）。
3. 选择 Emby 或 Jellyfin，扫描局域网或手动填写地址后登录。
4. 登录成功后进入首页，用方向键浏览，确认键播放。

**桌面端**

1. 从 [Harbor Releases](https://github.com/envyafish/Harbor/releases) 下载最新 `.dmg`（macOS）或 Windows 安装包 / 压缩包。
2. 打开 Harbor，填写服务器地址、用户名与密码登录。

若需手动准备字幕生成模型（Sidecar），见 [手动下载教程](https://github.com/envyafish/Harbor/blob/master/docs/MANUAL_SIDECAR_MODELS.md)。

---

## 隐私与安全

- 账号与访问令牌保存在系统钥匙串（桌面）或本机安全存储（电视）。
- Harbor 只连接**你自己的**媒体服务器，不需要 Harbor 云账号。
- 若启用弹幕，请求仅发往**你配置的**弹幕服务器；本应用不支持发送弹幕。
- 儿童模式的 PIN 与看片记录只留在本机。
- 若连接 Trakt，仅把播放进度同步到你的 Trakt 账号。

---

## 反馈

欢迎通过 [GitHub Issues](https://github.com/envyafish/Harbor-Android-TV-Release/issues) 提交问题与功能建议。

桌面版见 [Harbor](https://github.com/envyafish/Harbor)。本项目不开放源代码。

---

## 许可证

专有软件，保留所有权利。

---

## 致谢

- [Emby](https://emby.media/)
- [Jellyfin](https://jellyfin.org/)
- [极影视](https://www.zspace.cn/)
- [Media3 / ExoPlayer](https://developer.android.com/media/media3)
- [mpv](https://mpv.io/) / libmpv
- [Tauri](https://tauri.app/)
- [danmu_api](https://github.com/huangxd-/danmu_api) 及兼容弹幕服务
- [弹弹play](https://www.dandanplay.com/) 开放平台（协议兼容）
- [Trakt](https://trakt.tv/)
