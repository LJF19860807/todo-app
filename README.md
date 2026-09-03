# 待办事项 · 轻量 PWA

万事尽头，终将如意；一件一件，慢慢来。

## 功能

- ✅ 添加 / 勾选 / 删除任务
- 📅 待办日期 + 完成日期 + 完成用时
- 🎯 优先级（紧急 / 重要 / 一般）
- 💼 分类（工作 / 生活 / 学习 / 其他）
- 📌 置顶、🔍 搜索、📊 完成率统计
- 📝 备注（自动保存）、✏️ 双击编辑任务
- 💾 / 📂 导出 / 导入 JSON 备份
- 📲 安装到主屏幕（安卓 Chrome/Edge；iOS Safari）
- 📴 离线可用（Service Worker 缓存）

## 技术方案

- 纯前端，**无后端**，数据全部存在浏览器 `localStorage`
- PWA：`manifest.json` + `sw.js` 离线缓存
- 换机 / 清浏览器数据前：先「导出备份」，再用「导入恢复」

## 本地运行

双击 `start-server.bat`（或 `python -m http.server 8080`），打开 http://localhost:8080

## 手机安装

1. 手机用 **Chrome / Edge / Safari** 打开线上网址
2. 点页面里的「📲 安装到主屏幕」按钮（浏览器支持时自动显示）
3. 安卓 Chrome / Edge 会弹出安装窗口；iOS Safari 需用「分享 → 添加到主屏幕」

> 微信 / QQ 内置浏览器没有安装功能，请用系统浏览器打开。

## 图标生成

`node create-pwa-icons.js`（依赖 sharp）
