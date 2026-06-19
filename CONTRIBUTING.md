# 贡献指南

感谢你对 MD2WeChat Pro 的关注！欢迎提交 Issue 和 Pull Request。

## 🐛 提交 Issue

- 在提交新 Issue 前，请先搜索是否已有类似问题
- 请包含以下信息：
  - 问题描述
  - 复现步骤
  - 浏览器和操作系统
  - 截图（如有）

## 🔀 提交 Pull Request

1. Fork 本仓库
2. 创建功能分支：`git checkout -b feature/your-feature-name`
3. 提交更改：`git commit -m 'feat: add your feature'`
4. 推送分支：`git push origin feature/your-feature-name`
5. 提交 Pull Request

### Commit 规范

- `feat:` 新功能
- `fix:` 修复 Bug
- `style:` 样式调整（不影响功能）
- `docs:` 文档更新
- `refactor:` 重构
- `chore:` 构建/工具相关

## 🎨 新增模板

如果你想添加新的模板风格，在 `index.html` 中的 `TEMPLATES` 对象里添加一个新的配置即可：

```javascript
your_template: {
  name: '模板名称',
  primaryColor: '#hexcolor',
  secondaryColor: '#hexcolor',
  textColor: '#hexcolor',
  linkColor: '#hexcolor',
  codeBg: '#hexcolor',
  codeColor: '#hexcolor',
  preBg: '#hexcolor',
  blockquoteBg: '#hexcolor',
  blockquoteColor: '#hexcolor',
  h2Style: 'border-left',  // border-left | center | gradient | underline | plain
  tableHeadColor: '#hexcolor',
  fontFamily: 'system',    // system | serif | sans-serif | monospace
  paragraphAlign: 'left', // left | center | justify
  lineHeight: 1.75,
  letterSpacing: 0.5,
}
```

## 💻 本地开发

```bash
git clone https://github.com/yourname/md2wechat.git
cd md2wechat
open index.html
```

无需安装任何依赖，用浏览器直接打开 `index.html` 即可开发调试。

## 📋 代码规范

- JavaScript 使用 ES6+ 语法
- 缩进使用 2 个空格
- 注释用中文或英文，保持一致
