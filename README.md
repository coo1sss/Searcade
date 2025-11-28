🎮 Searcade 自动保号脚本
自动登录 Searcade 账号，防止因长期不登录而被删除。每 15 天自动运行一次。
🚀 使用方法
1. Fork 本仓库
2. 配置 Secrets
进入仓库 Settings → Secrets and variables → Actions，添加以下 secrets：
Secret 名称说明必需SEARCADE_ACCOUNTS账号信息（JSON格式）✅ 必需TELEGRAM_BOT_TOKENTelegram Bot Token⭕ 可选TELEGRAM_CHAT_IDTelegram Chat ID⭕ 可选
SEARCADE_ACCOUNTS 格式：
单个账号：
json[
  {"username": "your_username", "password": "your_password"}
]
多个账号：
json[
  {"username": "user1", "password": "pass1"},
  {"username": "user2", "password": "pass2"}
]
3. 启用 Actions
进入 Actions 标签页，启用工作流，点击 Run workflow 测试运行。
📸 查看结果

日志：Actions 页面查看运行日志
截图：运行完成后，在页面底部 Artifacts 下载 login-screenshots
通知：配置 Telegram 后会收到通知

⚙️ 自动运行
默认每 15 天自动运行一次，也可以手动触发。
