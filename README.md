<p align="center"><img src="docs/img/icon.png" width="96" alt="LitePlay"></p>

# 轻播 LitePlay

A clean Android video player · 一个干净的安卓视频播放器：本地视频、m3u8 / mp4 链接、外挂字幕、续播，开箱即用。不带内容、不收集数据。

**Download / 下载**：[LitePlay-1.1.0.apk](https://github.com/CodeHYY/liteplay/releases/download/v1.1.0/LitePlay-1.1.0.apk)（1.9 MB，Android 8.0+）· [Landing page](https://codehyy.github.io/liteplay/)

<p><img src="docs/img/home.jpg" width="170"> <img src="docs/img/play2.jpg" width="170"> <img src="docs/img/speed.jpg" width="170"> <img src="docs/img/pip.jpg" width="170"></p>

## English summary
- Plays local files, http(s) links, HLS (m3u8) and DASH; external .srt/.vtt subtitles; resume playback.
- Privacy: only the `INTERNET` permission, no analytics SDK, no account, no uploads. Ships with no media content.
- Free: speed 0.25×–2×, 5 resume entries, a 5-second ad every 3rd playback + banner. VIP (one-time offline license key): no ads, picture-in-picture, up to 4× speed, 200 resume entries.
- Verify: `shasum -a 256 LitePlay-1.1.0.apk` → `b5cfd049969e1fd5f8afeffdcbdf62b39f010fd6edf07445d2eee3b8847386eb`.

## 功能

| | 免费版 | VIP |
|---|---|---|
| 本地视频 / http(s) 链接 / HLS(m3u8) / DASH | ✅ | ✅ |
| 外挂字幕 (.srt / .vtt) | ✅ | ✅ |
| 断点续播 | ✅ 保留最近 5 条 | ✅ 保留最近 200 条 |
| 倍速 | 0.25×–2× | 0.25×–4× |
| 画中画小窗（按 Home 自动小窗） | ❌ | ✅ |
| 广告 | 每 3 次播放 1 条 5 秒广告 + 首页横幅 | 无广告 |

## 下载

在 [Releases](../../releases/latest) 下载 `LitePlay-*.apk`，安装时按系统提示允许“安装未知来源应用”。需要 Android 8.0+。

校验：`shasum -a 256 LitePlay-1.1.0.apk` 应与 Release 说明里的 SHA-256 一致。

## 隐私

- 不申请通讯录、定位、相机、麦克风、存储权限（本地视频通过系统文件选择器授权）。
- 只有 `INTERNET`：播放你填写的网络链接时才联网。
- 无统计 SDK、无账号、无上传。播放历史只保存在本机。

## 开通 VIP

App 内「激活 / 开通 VIP」输入授权码即可，授权码离线校验（ECDSA 签名），不需要联网、不需要账号。
购买方式见 App 内「购买」按钮。

## 声明

轻播只是播放器，不提供、不内置任何影视内容。请只播放你有权观看的内容。本页文案由 AI 辅助撰写。截图中的演示视频：Big Buck Bunny © Blender Foundation，CC-BY 3.0。

## 1.1.0 说明 / Notes
- 广告位内容来自 `https://codehyy.github.io/liteplay/ads.json`（只接受 https 链接；读取失败时显示自家 VIP 广告，不影响播放）。这是 App 唯一的后台请求，不上传任何用户数据。/ The app's only background request is a plain GET of that ads.json; nothing is uploaded.
- VIP 为年卡（1 年），只解锁功能，不含任何影视内容，也不保证第三方链接可用。/ VIP is a 1-year license that unlocks features only; no content is provided or guaranteed.
