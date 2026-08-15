AI 智能记账本 PWA

部署：
1. 将本文件夹完整上传到任意 HTTPS 静态托管服务。
2. 推荐：GitHub Pages / Vercel / Cloudflare Pages。
3. 用 iPhone Safari 打开部署后的网址。
4. 分享 → 添加到主屏幕。
5. 之后从 Home Screen 打开，即为独立 PWA。

Shortcut 写入：
支持 ?payload=<URL编码后的JSON>

示例 JSON：
{
  "date":"2026-08-15",
  "type":"Expense",
  "amount":28.5,
  "category":"Food",
  "merchant":"麦当劳",
  "account":"支付宝",
  "note":"午餐"
}

数据说明：
- 账单保存在该设备的 IndexedDB，同时镜像到 localStorage。
- 页面支持离线打开。
- iPhone 与 Mac 的本地数据库默认独立，不自动同步。
- iPhone 不能直接从 ZIP 安装 PWA；必须先部署到 HTTPS，再添加到主屏幕。
