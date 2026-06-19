# 📝 MD2WeChat Pro

> Markdown 转微信公众号排版工具 — 纯前端，无需后端，可视化样式调整，一键复制到公众号编辑器。

📄 中文 | [English](./README_EN.md)

## 🎯 解决什么问题

微信公众号编辑器不支持 Markdown，手动排版费时费力。本工具将 Markdown 一键转换为微信公众号兼容的富文本，**所有样式自动转为 inline**，复制后直接粘贴到公众号编辑器即可，格式不丢失。

## ✨ 特性

- 📝 **实时预览** — 左侧编辑 Markdown，右侧实时渲染微信效果
- 🎨 **10 套内置模板** — 微信经典绿、商务蓝、优雅紫、活力橙、极简灰、科技暗黑、文艺范、粉色少女、中国红、学术严谨
- 🎛️ **可视化样式面板** — 颜色选择器、字号滑块、行高滑块、字间距滑块、段落对齐、字体族、H2 风格，选择即生效
- 🎲 **随机配色** — 一键随机生成配色方案
- 💾 **方案保存/加载** — 将样式配置保存为 JSON，支持导入导出和本地存储
- 📋 **一键复制** — 所有样式自动 inline，直接粘贴到公众号编辑器
- 📥 **导入 .md 文件** — 支持导入本地 Markdown 文件
- 📤 **导出 HTML** — 导出包含代码高亮的完整 HTML 文件
- ⌨️ **快捷键** — `Cmd/Ctrl+S` 或 `Cmd/Ctrl+Enter` 快速复制
- 📱 **响应式** — 移动端也可使用

## 🚀 快速开始

### 在线使用

直接用浏览器打开 `index.html` 即可，无需安装任何依赖。

```bash
git clone https://github.com/yourname/md2wechat.git
cd md2wechat
open index.html   # macOS
# 或直接双击 index.html 用浏览器打开
```

### 使用流程

1. 在左侧编辑器输入 Markdown 内容
2. 点击模板选择条，选择喜欢的风格
3. （可选）切换到「样式设置」标签页，可视化调整颜色和排版
4. 点击「📋 复制」按钮
5. 粘贴到微信公众号编辑器，完成！

## 📸 截图

![MD2WeChat Pro 界面](./screenshot.png)

## 🎨 内置模板

| 模板 | 主色 | 风格 | 适用场景 |
|------|------|------|---------|
| 微信经典绿 | `#07c160` | 清新自然 | 通用文章 |
| 商务蓝 | `#1990ff` | 专业稳重 | 商务报告 |
| 优雅紫 | `#6222c2` | 优雅气质 | 生活方式 |
| 活力橙 | `#ff7a45` | 活力满满 | 营销推广 |
| 极简灰 | `#555555` | 极简主义 | 技术文档 |
| 科技暗黑 | `#00d4aa` | 酷炫暗色 | 技术教程 |
| 文艺范 | `#8b6914` | 复古文艺 | 散文随笔 |
| 粉色少女 | `#ec4899` | 甜美可爱 | 生活分享 |
| 中国红 | `#c0392b` | 大气庄重 | 节日主题 |
| 学术严谨 | `#2c3e50` | 严谨正式 | 论文报告 |

## 🎛️ 可调样式

### 颜色（颜色选择器 + 十六进制输入）

- 主色调 / 背景辅色 / 正文颜色 / 链接颜色 / 引用文字颜色
- 代码背景 / 代码文字 / 代码块背景
- 引用背景 / 表头颜色

### 排版（滑块 + 下拉）

- 正文字号（12px ~ 22px）
- 行高（1.4 ~ 2.2）
- 字间距（0 ~ 3px）
- 段落对齐（左对齐 / 居中 / 两端对齐）
- 字体族（系统默认 / 衬线 / 无衬线 / 等宽）
- H2 标题风格（左边框竖线 / 居中下划线 / 渐变背景 / 底部粗线 / 纯文字）

## 💾 方案管理

- **保存方案** — 将当前样式配置保存为 JSON，存储到浏览器 localStorage
- **加载方案** — 从本地存储加载，或粘贴 JSON 导入
- **导入/导出** — 复制 JSON 分享给他人，或从他人处导入

## ⚠️ 技术说明

### 为什么所有样式都是 inline？

微信公众号编辑器会过滤掉 `<style>` 标签和 `class` 属性，只保留 `style="..."` 内联样式。因此本工具的核心逻辑是将所有 CSS 样式自动转换为 inline style，确保粘贴后格式不丢失。

### 技术栈

- [marked.js](https://github.com/markedjs/marked) — Markdown 解析
- [highlight.js](https://github.com/highlightjs/highlight.js) — 代码语法高亮
- 纯 HTML + CSS + JavaScript，无框架依赖，无后端

### 浏览器兼容

- Chrome / Edge / Safari / Firefox 最新版
- 推荐使用 Chrome 获得最佳体验

## 📁 项目结构

```
md2wechat/
├── index.html          # 主应用（单文件，含全部代码）
├── README.md           # 中文说明
├── README_EN.md        # English README
├── LICENSE             # MIT License
├── CONTRIBUTING.md     # 贡献指南
├── CHANGELOG.md        # 更新日志
├── .gitignore
└── examples/
    └── sample.md       # 示例 Markdown 文件
```

## 🤝 贡献

欢迎提交 Issue 和 PR！详见 [CONTRIBUTING.md](./CONTRIBUTING.md)。

## 📄 License

[MIT License](./LICENSE) — 可自由使用、修改、分发。

## 🙏 致谢

- [marked.js](https://github.com/markedjs/marked) — Markdown 解析库
- [highlight.js](https://github.com/highlightjs/highlight.js) — 代码语法高亮库
- 所有为微信公众号排版做出贡献的开源项目
