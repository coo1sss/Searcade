Searcade 自动保号脚本

自动登录 Searcade 账号，防止因长期不登录而被删除。每 7 天自动运行一次。

配置 Secrets

进入仓库 Settings → Secrets and variables → Actions，添加以下 secrets：

必需配置：

SEARCADE_ACCOUNTS - 账号信息（JSON格式）

可选配置：

TELEGRAM_BOT_TOKEN - Telegram Bot Token

TELEGRAM_CHAT_ID - Telegram Chat ID

SEARCADE_ACCOUNTS 格式示例：

单个账号：

[{"username": "your_username", "password": "your_password"}]

多个账号：

[{"username": "user1", "password": "pass1"}, {"username": "user2", "password": "pass2"}]

3. 启用 Actions

进入 Actions 标签页，启用工作流，点击 Run workflow 测试运行。

查看结果

日志：Actions 页面查看运行日志

截图：运行完成后，在页面底部 Artifacts 下载 login-screenshots

通知：配置 Telegram 后会收到通知

自动运行

默认每 7 天自动运行一次，也可以手动触发。

