# Glyphids · We Hear You

**Across the dark, someone is listening.**

A quiet correspondence puzzle set aboard a Deep Sky Survey receiving station. Read an unfamiliar language, compare signals, and find a voice on the other side of the stars.

[Play Glyphids](https://glyphids.ender-wiggin.com)

[![Buy Me a Coffee](https://img.shields.io/badge/Buy_Me_a_Coffee-enderwiggin-5F3AA6?style=for-the-badge&logo=buymeacoffee&logoColor=white)](https://buymeacoffee.com/enderwiggin)

## 游戏

在深空巡天的接收站里，读懂一种陌生的语言，和遥远的奈里通信。

- 紫白色办公桌面，可拖动、缩放和堆叠应用窗口。
- 信号分析、词典、邮件和笔记共同构成解谜过程。
- 中英文界面、本地存档，以及可导出的 PNG 纪念图。
- 推荐使用电脑；手机建议横屏，保持相同的桌面交互方式。

存档保存在当前浏览器中。换设备或清理浏览器数据前，请在设置中导出存档。

## Repository

This repository contains the **built static release** only:

```text
README.md
dist/
```

The development source, dependencies, credentials, and test artifacts are not included. The game is inspired by the Glyphids from SETI: Search for Extraterrestrial Intelligence; it is an independent fan project, not an official SETI product.

## Run locally

Serve `dist` with any static HTTP server. For example, with Python installed:

```sh
python3 -m http.server 8080 --directory dist
```

Open <http://localhost:8080>. Browser storage is specific to each origin, so a local save is separate from the live website.

## Deployment

The published site is hosted on Cloudflare Workers Static Assets at **https://glyphids.ender-wiggin.com**.

Subsequent releases should upload the updated `dist` using the development project's Wrangler configuration, which includes the `glyphids.ender-wiggin.com` custom-domain binding. Preserve that binding when deploying. GitHub is the release archive; pushing a commit alone does not automatically publish a new Cloudflare version.

## Support

If this small signal reached you, [buy me a coffee](https://buymeacoffee.com/enderwiggin).
