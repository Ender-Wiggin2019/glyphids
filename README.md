# Glypyids

**Across the dark, someone is listening.**

A quiet correspondence puzzle set at a Deep Sky Survey receiving station in 2147. Humanity is reaching further into space. On your first shift, a repeating signal arrives. Read its pictures, mark unfamiliar symbols, and find the words to write back.

[Play Glyphids](https://glyphids.ender-wiggin.com)

[![Buy Me a Coffee](https://img.shields.io/badge/Buy_Me_a_Coffee-enderwiggin-5F3AA6?style=for-the-badge&logo=buymeacoffee&logoColor=white)](https://buymeacoffee.com/enderwiggin)

## 游戏

2147 年，人类正在走向更远的太空。你在深空巡天接收站值班的第一天，收到了一段重复信号。看图、标注字符、拼出单词，然后写一封回信。

- Deep Sky Survey 品牌桌面，原创机构标志与 slogan；可拖动、缩放和堆叠应用窗口。
- 数据分析器（Data Analyzer）采用白蓝配色，Scan 采用紫色；应用使用 SETI v2 图标。
- 从简单标注开始，随 Ender 的邮件逐步学习图像、词长和上下文之间的关系。
- SeNews 太空探索日报配有原创概念插画；新闻随时间与进度安静更新，报道多个太空机构的探索，描绘这个寻找外星邻居的时代。
- 信号分析、词典、邮件和笔记共同构成解谜过程；图中的数字标签也可以独立破译，破译表实时汇总当前有效标注，支持修改、撤销、重做与刷新恢复。
- 词典提供数学与分子式参考；计算器支持精确的双向进制转换。
- 邮件、监测备注和记事本支持文字与 Glyph 混排；私人备注保留在记事本。
- 抽屉式键盘；实体键盘支持字母和数字，Glyph 字符通过屏幕键盘输入。
- 人物回复通过邮件发送，逐级帮助位于设置。
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
