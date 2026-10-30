# Glypyids

**Across the dark, someone is listening.**

A quiet correspondence puzzle set at a Deep Sky Survey receiving station in 2147. You and your colleague Ender are studying a repeating signal. Read its pictures, annotate unfamiliar symbols, and build the mapping needed for humanity's first reply.

[Play Glyphids](https://glyphids.ender-wiggin.com)

[![Buy Me a Coffee](https://img.shields.io/badge/Buy_Me_a_Coffee-enderwiggin-5F3AA6?style=for-the-badge&logo=buymeacoffee&logoColor=white)](https://buymeacoffee.com/enderwiggin)

## 游戏

2147 年，你和同事 Ender 在深空巡天接收站收到了一段重复信号。从图中的八个数字开始，标注字符、辨认图像，整理出人类第一次回应所需的映射。

- Deep Sky Survey 品牌桌面，原创机构标志与 slogan；可拖动、缩放和堆叠应用窗口。
- 数据分析器（Data Analyzer）采用白蓝配色，Scan 采用紫色；应用使用 SETI v2 图标。
- 标注会自动同步给 Ender；阅读来信，逐步接收更清晰的图像与新信号。
- SeNews 太空探索日报配有原创概念插画；新闻随时间与进度安静更新，报道多个太空机构的探索，描绘这个寻找外星邻居的时代。
- 信号分析、词典、邮件和笔记共同构成解谜过程；图中的数字标签也可以独立破译，破译表实时汇总当前有效标注，支持修改、撤销、重做与刷新恢复。
- 词典使用分类 Tab，并覆盖主线中的每个单词；计算器支持精确的双向进制转换。星图软件提供常见星座的图形、英文名称和介绍。
- 正确标注会显示对应中文译文；记事本支持文字与 Glyph 混排。
- 抽屉式键盘；实体键盘支持字母和数字，Glyph 字符通过屏幕键盘输入。
- Ender 的邮件给出观察方向，卡关时会有新线索。整理好映射后，通过独立的信号发射器完成第一次通信。
- 中英文界面、本地存档，以及可导出的 PNG 纪念图。
- 支持电脑、手机横屏与竖屏，保持相同的桌面交互方式。

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

Subsequent releases should upload the updated `dist` using the development project's Wrangler configuration, which includes the `glyphids.ender-wiggin.com` custom-domain binding. Preserve that binding when deploying. GitHub is the release archive; pushing a commit alone does not automatically publish a new Cloudflare version. Retain the hashed JavaScript and CSS from earlier releases so open tabs can still load their applications; the development project provides `prepare:release` for this step.

## Support

If this small signal reached you, [buy me a coffee](https://buymeacoffee.com/enderwiggin).
