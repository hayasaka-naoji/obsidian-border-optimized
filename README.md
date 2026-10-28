# Border Optimized

一个以 [Border](https://github.com/Akifyss/obsidian-border) 为基础的 Obsidian 主题改版：更安静的磨砂玻璃背景、更适合中文长文阅读的排版，以及更克制的标签页与动效。

A refined fork of the [Border](https://github.com/Akifyss/obsidian-border) theme for Obsidian: quieter frosted-glass backgrounds, typography tuned for long-form reading (including CJK), and more restrained tabs and motion.

> 版本 Version: **1.13.9** · 最低 Obsidian 版本 Min app version: **0.16.0**

## 安装 Installation

1. 下载本仓库，或克隆到你的库中：
   ```bash
   git clone https://github.com/hayasaka-naoji/obsidian-border-optimized.git \
     "<你的库>/.obsidian/themes/Border Optimized"
   ```
2. 打开 Obsidian → **设置 → 外观 → 主题**，选择 **Border Optimized**。
3. 若样式未刷新，重启 Obsidian 或在主题列表中重新选择一次。

也可以直接复制 `manifest.json` 与 `theme.css` 到 `<库>/.obsidian/themes/Border Optimized/` 目录。

## 相对上游的改动 Changes

### 默认外观
- 默认开启自动隐藏：底部状态栏、左侧功能区、侧边面板头部按钮、标签页标题栏。
- 默认开启亮色 / 暗色卡片布局。
- 面板背景默认使用 CSS 磨砂玻璃样式，而非 `background-primary`。

### 背景与材质
- 磨砂玻璃层叠加一层低强度 SVG 噪点纹理（`feTurbulence`），减少大面积模糊的塑料感。
- 底层背景由高饱和的多层网格渐变改为低饱和径向渐变 + `background-tertiary`，视觉更安静。
- 亮色模式文字层级略微加深（muted / faint），暗色模式 faint 略微提亮。
- 阴影整体减淡，边框透明度微调。

### 排版
- 新增现代无衬线字体栈，包含 PingFang SC / 微软雅黑 / Noto Sans CJK 回退，且仍尊重 Obsidian 的字体覆盖设置。
- 标题字号：H1 1.7em、H2 1.45em、H3 1.25em、H4 1.15em、H5 1.075em、H6 1em；H2 / H6 字重调整为 700 / 600。
- 正文行高 1.65，阅读模式段落间距 0.9em，列表间距 0.1em。
- 标题增加上方留白、收紧下方间距，形成更清晰的标题节奏。

### 界面细节
- 标签页改为透明激活背景 + 底部圆角强调色下划线，去掉凸起块与内阴影。
- 卡片布局的面板间距由 16px 收紧为 8px。
- 自动隐藏的进入 / 退出动画改为更细腻的 `cubic-bezier` 缓动。

## 许可 License

基于 Akifyss 的 [obsidian-border](https://github.com/Akifyss/obsidian-border)，遵循 MIT License。

- Copyright (c) 2022 Akifyss（原始主题）
- Copyright (c) 2026 Hayasaka（本改版）

完整条款见 [LICENSE](LICENSE)。
