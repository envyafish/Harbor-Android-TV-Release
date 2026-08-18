# Harbor TV

[中文](README.md) | **English**

An **Android TV / Google TV** client for [Emby](https://emby.media/) and [Jellyfin](https://jellyfin.org/).

Harbor TV is built for the living room: browse your libraries full-screen, continue where you left off, do everything with a D-pad, and play with embedded **Media3 / ExoPlayer**. Optional danmaku is available from danmu_api–compatible sources you configure yourself (view only).

[Telegram group](https://t.me/HarborRelease)

---

## Purchase

Buy Harbor from the [shop](https://pay.ldxp.cn/shop/767OK1ZS):

<img src="docs/shop.png" alt="Shop QR code" width="220" />

The TV app uses the same Harbor Pro license as the desktop app. After activation, sign in to your own media server.

---

## Screenshots

### Home

![Home](docs/screenshots/home.png)

### Library

![Library](docs/screenshots/library.png)

### Detail

![Detail](docs/screenshots/detail.png)

### Player

![Player](docs/screenshots/player.png)

---

## Features

- **Living-room UI** — full-screen hero plus poster rows; no persistent sidebar
- **Continue watching** — resume playback; series show the episode that will play next
- **Libraries** — grid from the home row, with unwatched / watched / favorite filters
- **Search & favorites** — system IME search; favorites grouped by library
- **Details** — backdrop, play / resume, seasons, episodes, and cast
- **Native playback** — Direct Play first, transcode if needed
- **Subtitles & danmaku** — server subtitle tracks; danmaku is view-only, with multiple sources
- **Trakt** — device-code connect, then scrobble progress (no calendar or watchlist sync)
- **Child mode** — pin a child account, local PIN, daily time limit, local watch log for parents
- **Multiple accounts** — several Emby / Jellyfin servers and users; add another user on the same server without retyping the address

---

## Platforms

| Platform | Notes |
|----------|--------|
| Android TV / Google TV | D-pad, confirm, and back; touch is not a target |
| Android 7 or later (API 24+) | API 28+ devices recommended |

Install on a **TV or TV box**. This is not a phone or tablet app.

---

## Supported media servers

| Server | Notes |
|--------|--------|
| [Emby](https://emby.media/) | Primary target |
| [Jellyfin](https://jellyfin.org/) | Supported |

---

## Requirements

- An Emby / Jellyfin server you can reach
- An activated Harbor Pro license
- An Android TV or Google TV device (Android 7+)
- Network access to your server (usually the same LAN)

---

## Getting started

1. Download the latest APK from [Releases](https://github.com/envyafish/Harbor-Android-TV-Release/releases) and install it from a USB drive or with `adb install`.
2. Activate Harbor Pro on first launch (scan the on-screen QR from a phone on the same Wi‑Fi and submit the key).
3. Add Emby or Jellyfin: scan the LAN, or type the server address and sign in.
4. After login you land on Home. Move with the D-pad and press confirm to play.

---

## Privacy

- Credentials and access tokens stay on the device.
- Harbor TV talks to **your** media server only. There is no Harbor cloud account.
- If you enable danmaku, requests go only to **the danmaku servers you configure**. Sending danmaku is not supported.
- If you connect Trakt, only playback progress is sent to your Trakt account.

---

## Feedback

Please file issues and ideas on [GitHub Issues](https://github.com/envyafish/Harbor-Android-TV-Release/issues).

The desktop app lives at [Harbor](https://github.com/envyafish/Harbor). This project is not open source.

---

## License

Proprietary software. All rights reserved.

---

## Acknowledgements

- [Emby](https://emby.media/)
- [Jellyfin](https://jellyfin.org/)
- [Media3 / ExoPlayer](https://developer.android.com/media/media3)
- [danmu_api](https://github.com/huangxd-/danmu_api) and compatible danmaku services
- [Dandanplay](https://www.dandanplay.com/) open platform (protocol compatibility)
- [Trakt](https://trakt.tv/)
