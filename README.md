# Harbor TV（港湾电视版）

面向 [Emby](https://emby.media/) / [Jellyfin](https://jellyfin.org/) 的 **Android TV / Google TV** 客户端。

Harbor TV 给客厅用：全屏浏览媒体库、继续观看，用遥控器完成全部操作，并通过内嵌 **Media3 / ExoPlayer** 播放。可选接入你自行配置的、兼容 danmu_api 协议的弹幕源（只看不发）。

[TG 交流群](https://t.me/HarborRelease)

---

## 购买

可通过[店铺](https://pay.ldxp.cn/shop/767OK1ZS)购买 Harbor：

<img src="docs/shop.png" alt="店铺二维码" width="220" />

电视端与桌面端共用同一套 Harbor Pro 许可证。激活后即可登录你自己的媒体服务器。

---

## 截图

### 首页

![首页](docs/screenshots/home.png)

### 媒体库

![媒体库](docs/screenshots/library.png)

### 详情

![详情](docs/screenshots/detail.png)

### 播放器

![播放器](docs/screenshots/player.png)

---

## 功能

- **客厅全屏** — 大背景推荐 + 海报行，无常驻侧栏；方向键即可浏览
- **继续观看** — 断点续播；剧集会标出即将播放的集数
- **媒体库** — 从首页进网格，筛选未看 / 已看 / 收藏，按年份、类型排序
- **搜索 / 收藏** — 系统输入法搜索；收藏页按媒体库分组
- **详情** — 全屏背景、播放 / 续播、季集与演职员
- **原生播放** — 优先 Direct Play，失败再由服务器转码
- **字幕与弹幕** — 服务器字幕轨；弹幕只看不发，可配置多个弹幕源
- **Trakt** — 设备码连接后同步播放进度（无日历 / 想看对账）
- **儿童模式** — 指定儿童账号、本机 PIN、每日时长；家长可看本机看片记录
- **多账号** — 多台 Emby / Jellyfin、多个用户，同一服务器可直接加账号

---

## 支持平台

| 平台 | 说明 |
|------|------|
| Android TV / Google TV | 遥控器方向键、确认、返回；触控不是目标 |
| Android 7 及以上（API 24+） | 建议 API 28+ 的设备 |

请安装到 **电视机或电视盒子**，不要当作手机 / 平板应用使用。

---

## 支持的媒体服务器

| 服务器 | 说明 |
|--------|------|
| [Emby](https://emby.media/) | 主要支持目标 |
| [Jellyfin](https://jellyfin.org/) | 已支持 |

---

## 环境要求

- 可访问的 Emby / Jellyfin 服务器
- 已激活的 Harbor Pro 许可证
- Android TV 或 Google TV 设备（Android 7+）
- 同一局域网或可访问服务器的网络

---

## 开始使用

1. 从 [Releases](https://github.com/envyafish/Harbor-Android-TV-Release/releases) 下载最新 APK，用电视的「从 U 盘安装」或 `adb install` 装上。
2. 首次打开先激活 Harbor Pro（可用手机扫激活页二维码，在同一 Wi‑Fi 下提交许可证）。
3. 添加 Emby 或 Jellyfin：可扫局域网，或手动填写服务器地址后登录。
4. 登录成功后进入首页，用方向键浏览，确认键播放。

---

## 隐私与安全

- 账号与访问令牌保存在本机。
- Harbor TV 只连接**你自己的**媒体服务器，不需要 Harbor 云账号。
- 若启用弹幕，请求仅发往**你配置的**弹幕服务器；本应用不支持发送弹幕。
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
