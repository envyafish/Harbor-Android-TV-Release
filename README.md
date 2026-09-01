<div align="center">

<img src="docs/logo.png" width="120" height="120" alt="Harbor TV">

# Harbor TV（港湾电视版）

**面向 [Emby](https://emby.media/) / [Jellyfin](https://jellyfin.org/) 的 Android TV / Google TV 客户端**

[![电视版](https://img.shields.io/github/v/release/envyafish/Harbor-Android-TV-Release?style=flat-square&label=tv)](https://github.com/envyafish/Harbor-Android-TV-Release/releases/latest)
[![桌面版](https://img.shields.io/github/v/release/envyafish/Harbor?style=flat-square&label=desktop)](https://github.com/envyafish/Harbor/releases/latest)
[![Downloads](https://img.shields.io/github/downloads/envyafish/Harbor-Android-TV-Release/total?style=flat-square)](https://github.com/envyafish/Harbor-Android-TV-Release/releases)

[下载](https://github.com/envyafish/Harbor-Android-TV-Release/releases/latest) · [桌面端 Harbor](https://github.com/envyafish/Harbor) · [反馈 Bug](https://github.com/envyafish/Harbor-Android-TV-Release/issues) · [购买](https://pay.ldxp.cn/shop/767OK1ZS) · [TG 交流群](https://t.me/HarborRelease)

</div>

---

客厅版 Harbor，运行在 **Android TV / Google TV**。全屏沉浸、方向键操作，浏览与播放习惯与桌面端对齐，但按遥控重新做了交互。

桌面端见 [Harbor](https://github.com/envyafish/Harbor)（macOS / Windows，内嵌 **libmpv**）。

需要 Harbor Pro 激活后使用。可用遥控器粘贴许可证，也可扫局域网二维码在手机 / 电脑上提交。

---

## 购买

可通过 [店铺](https://pay.ldxp.cn/shop/767OK1ZS) 购买 Harbor Pro。同一许可证可用于桌面端与 Harbor TV。

<img src="docs/shop.png" alt="店铺二维码" width="220" />

---

## 首页

满屏 Backdrop + 顶部横行挑片。有继续观看时，Hero 合并续看与 Next Up；焦点移动时背景、标题和「播放」按钮一起切换。往下是媒体库卡片，以及各库最新。

顶栏为 **首页 · 收藏 · 搜索**，右侧是账号、儿童模式与设置。

<img src="docs/screenshots/home.png" alt="Harbor TV 首页" width="100%" />

<img src="docs/screenshots/home-libraries.png" alt="Harbor TV 媒体库行" width="100%" />

---

## 媒体库

海报网格，可用全部 / 未看 / 已看 / 收藏 / 合集筛选，并按年份、类型、标题等排序。每个库会记住上次的筛选与排序。

<img src="docs/screenshots/library.png" alt="Harbor TV 媒体库网格" width="100%" />

---

## 详情

全宽背景、分辨率 / 时长 / 音轨信息，「继续」或从头播放，以及收藏、加入播放列表。音轨与字幕可在详情页选好再播。下方是演职员与相似影片。

<img src="docs/screenshots/detail.png" alt="Harbor TV 电影详情" width="100%" />

<img src="docs/screenshots/detail-similar.png" alt="Harbor TV 演职员与相似" width="100%" />

<img src="docs/screenshots/people.png" alt="Harbor TV 演职员页" width="100%" />

---

## 收藏与搜索

收藏按库分组。搜索页在未输入时展示服务器推荐，输入片名或剧名后自动出结果。

<img src="docs/screenshots/favorites.png" alt="Harbor TV 收藏" width="100%" />

<img src="docs/screenshots/search.png" alt="Harbor TV 搜索" width="100%" />

---

## 播放器

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

---

## 儿童模式

指定一个账号并设置 4 位 PIN。可分别限制工作日 / 周末每日时长，以及最早 / 最晚开播。家长可用 PIN 查看看片记录。儿童模式下没有设置、换号和弹幕入口。

<img src="docs/screenshots/kids.png" alt="Harbor TV 儿童模式设置" width="100%" />

<img src="docs/screenshots/watch-log.png" alt="Harbor TV 看片记录" width="100%" />

---

## 功能一览

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
| Harbor TV | Android TV / Google TV（Android 7+） | 遥控 / 方向键；需 Harbor Pro |
| [Harbor 桌面端](https://github.com/envyafish/Harbor) | macOS 26+ / Windows 10+（x64） | 内嵌 libmpv；与电视端共用许可证 |

请安装到 **电视机或电视盒子**，不要当作手机 / 平板应用使用。

---

## 支持的媒体服务器

| 服务器 | Harbor TV | 桌面端 |
|--------|-----------|--------|
| [Emby](https://emby.media/) | 主要支持 | 主要支持 |
| [Jellyfin](https://jellyfin.org/) | 已支持 | 已支持 |
| [极影视](https://www.zspace.cn/) | 不支持 | 兼容，缺乏充分测试 |

---

## 开始使用

1. 从 [Releases](https://github.com/envyafish/Harbor-Android-TV-Release/releases) 下载最新 APK，用电视的「从 U 盘安装」或 `adb install` 装上。
2. 用 Harbor Pro 许可证激活（可用遥控器粘贴，或扫码在手机 / 电脑上提交）。
3. 选择 Emby 或 Jellyfin，扫描局域网或手动填写地址后登录。
4. 登录成功后进入首页，用方向键浏览，确认键播放。

桌面端安装见 [Harbor](https://github.com/envyafish/Harbor)。

---

## 隐私与安全

- 账号与访问令牌保存在本机安全存储。
- Harbor TV 只连接**你自己的**媒体服务器，不需要 Harbor 云账号。
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
- [Media3 / ExoPlayer](https://developer.android.com/media/media3)
- [danmu_api](https://github.com/huangxd-/danmu_api) 及兼容弹幕服务
- [弹弹play](https://www.dandanplay.com/) 开放平台（协议兼容）
- [Trakt](https://trakt.tv/)
