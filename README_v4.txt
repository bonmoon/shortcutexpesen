AI 智能记账本 PWA v4 修复版

修复：
1. 新增交易确认后，Dashboard 自动切换到该交易所属月份，因此本月结余/收入/支出立即刷新。
2. Mobile Hero 增加前后月份切换按钮，避免查看错误月份。
3. 自定义 Agent 图片/GIF 会完全替换默认 Agent，不再出现一半默认、一半上传图。
4. Agent 增加“填满并裁切 / 完整显示”两种显示模式。
5. 主题配色升级为全局主题：页面背景、App 背景、卡片、Topbar、底部导航、输入框、确认卡和 AI 弹窗都会随主题变化。
6. Service Worker cache 升级为 v4。

部署：
覆盖 GitHub Pages 根目录 index.html / service-worker.js / manifest.webmanifest / icons。
重新打开 Home Screen PWA；若仍是旧版，请完全关闭 PWA 后再开，必要时清除该站点 Safari 网站数据后重新添加到主屏幕。
