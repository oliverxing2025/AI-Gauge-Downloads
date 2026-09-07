# 隐私说明 / Privacy

更新：2026-09-07。适用当前 Beta。开发者：小奥。

AI Gauge 不设自有数据接收服务器，不上传对话给开发者，不包含广告或遥测。请求目标服务时，对方仍可获取 IP 地址、请求时间等网络信息，并按其政策处理数据。

| 功能 | 读取与用途 | 保存及发送范围 |
| --- | --- | --- |
| Codex | 调用本机客户端读取额度、账户统计和邮箱；读取本机日志计算用量与任务状态 | 鉴权由 Codex 客户端管理；聚合结果/增量游标缓存在本机，不缓存对话正文；模型名称及用量会显示在界面 |
| Claude Code | 读取本机凭据文件或钥匙串的 OAuth 令牌 | 令牌仅在内存中用于 api.anthropic.com；不自行续期或保存该令牌 |
| Claude 桌面版 | 只读 Cookie 数据库，借助系统钥匙串解码会话 | 会话仅在内存中向 claude.ai 查询账户/工作区/额度；不复制数据库或持久化 Cookie |
| Grok | 读取本机 CLI 登录凭据 | 仅在内存用于 cli-chat-proxy.grok.com，不续期或保存令牌 |
| DeepSeek 余额 | 用户输入 API Key | 保存在本机钥匙串，用于 api.deepseek.com 的余额查询 |
| DeepSeek 用量 | 用户在内置官方平台页面登录，点击连接后提取平台令牌 | 使用临时 WebKit 会话；令牌保存在本机钥匙串，按 API Key 指纹区分，用于 platform.deepseek.com 用量查询；账号对应关系由用户选择确认 |
| 重置预报 | 查询 codex-reset.com 公共预测接口 | 不向该网站发送账号、令牌、日志或用量；公开预测可缓存在本机 |
| 名称、头像、设置 | 用户设置的本机显示资料和偏好 | 保存到本机偏好；头像缩小保存，不上传开发者 |

## 删除与控制

关闭 AI Gauge 可停止后台读取。DeepSeek 用量可在“连接 DeepSeek 用量”窗口断开；请先断开用量，再移除 API Key。历史密钥对应的旧令牌可在系统“钥匙串访问”中搜索 AI Gauge DeepSeek 并删除。Claude/Grok/Codex 的原有登录信息由其客户端管理，本应用不会删除。

本机缓存：~/Library/Caches/local.quotacat.macos；退出后可删除该目录。偏好可在退出后通过 `defaults delete local.quotacat.macos` 清除（包括自定义名称、头像和设置，不清除钥匙串凭据）。删除应用本身不会自动删除这些数据。

音频在本机离线播放。微信赞赏码在本机显示，应用不接收付款信息；扫码支付由微信处理。顶部可能显示邮箱，分享截图前请遮挡。统计可能包含本机不同账号时期的日志，不应当作当前账户独占统计。

## English

No developer telemetry or advertising is included. Credentials are read locally for the selected provider and sent only to its service. DeepSeek keys and platform tokens are stored in macOS Keychain; other provider credentials are not persisted by AI Gauge. Local usage aggregates, preferences and public forecast responses may be cached. The public forecast endpoint receives no account credentials or usage. Disconnect DeepSeek usage before removing its key; old entries can be deleted in Keychain Access. Deleting the app does not delete preferences, caches or Keychain entries. Network services may observe IP addresses and apply their own privacy policies.
