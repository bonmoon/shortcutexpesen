AI 智能记账本 PWA v2

本次更新：
- 手机端重新布局：安全区、紧凑 Dashboard、底部导航、移动端卡片尺寸。
- Shortcut payload 不再立即入账。
- 页面收到 payload 后先弹出紫色确认卡。
- 点击“确认记账”才写入 IndexedDB/localStorage；取消则不写入。

Shortcut 最后一段：
1. 保持原有 OCR → DeepSeek → JSON。
2. 将 JSON 做 URL Encode。
3. 最后 URL 改为：
   https://你的GitHubPages地址/?review=1&payload=[编码后的JSON]
4. 使用“打开 URL”。

GitHub 更新：
直接用本包里的 index.html / manifest.webmanifest / service-worker.js / icons 覆盖仓库根目录同名文件。
GitHub Pages 会自动重新部署。

注意：
iOS 系统通知/Show Alert 的颜色、圆角和字体由系统控制，不能自定义成紫色 UI。
本版本采用 PWA 内的确认卡实现同一视觉风格。
