# 🍇 TheBerryHost 每日自动签到

自动每天领取 TheBerryHost Discord 服务器的每日 BerryCoins 奖励。

## 使用方法

### 1. Fork 本仓库

点击右上角 **Fork** 按钮。

### 2. 设置 GitHub Secrets

进入你 Fork 后的仓库 → **Settings** → **Secrets and variables** → **Actions** → **New repository secret**

| Secret 名称 | 说明 | 获取方法 |
|-------------|------|----------|
| `DISCORD_TOKEN` | 你的 Discord 账号 Token | 打开 Discord 网页版 → F12 → Network → 任意请求 → Headers → `authorization` |
| `SESSION_ID` | 你的 Discord Session ID | F12 → Network → 找一个 `interactions` 请求 → Payload → `session_id` |

### 3. 启用 Actions

进入你的仓库 → **Actions** → 点击 **Enable** 启用工作流。

### 4. 运行

- **自动运行**：每天北京时间 09:00 自动执行
- **手动运行**：Actions → TheBerryHost 每日领取 → Run workflow

## ⚠️ 注意事项

- 本脚本仅供学习研究，使用前请了解 [Discord 服务条款](https://discord.com/terms)
- **请勿**将你的 `DISCORD_TOKEN` 泄露给任何人
- Secrets 在 GitHub 中是加密存储的，Fork 后他人无法看到你的配置
