# AI Gauge — Beta

macOS 菜单栏 AI 额度与用量工具。独立开发者：小奥。免费使用，源码暂不公开。

当前版本：**0.1.0 Beta · build 54**。

本版 Codex 的“本账户昨日估算”和“本账户当月估算”改用账户已上报的 Token，统一以 **$1 / 百万 Token** 参考折算，非实际账单或模型官方报价。按 UTC 日期累计，同账户相同数据在各电脑的结果一致。“昨日 Token”与昨日估算使用同一天的记录；昨日未上报时显示“待更新”，不使用本机日志补算。折算说明收纳在金额卡片的悬停提示中。

## 安装

要求 macOS 14+，安装包包含 Apple 芯片及 Intel 两种架构。双击 DMG，将 AI Gauge 拖入 Applications，从应用程序中打开，然后推出安装磁盘。应用出现在顶部菜单栏。请勿直接在 DMG 或同步中的应用包内运行。

当前为未公证的测试版，macOS 可能阻止首次打开。如果确认安装包来源可信，可按系统“隐私与安全”中的提示操作；不要关闭系统安全保护。正式签名、公证及 Intel/macOS 14 实机验收尚待完成。

## 功能范围

- Codex：本机已安装并登录客户端后读取额度、账户用量与本机日志统计；已有本机数据验证，仍需新电脑安装验收。
- Claude、Grok、DeepSeek：实验性接入。解析及模拟请求已测试，完整真实账号链路尚未全部验收；接口可能变化。
- Kimi、WorkBuddy：未启用。
- 本机费用是 API 等价估算，不是订阅账单；第三方重置预测仅供参考。
- 账号、密钥、日志和偏好不会随安装包同步，需要在每台 Mac 配置。

详见 PRIVACY.md、TERMS.md、THIRD_PARTY.md 和 CHANGELOG.md。反馈问题时请附版本、系统版本、芯片及复现步骤；先遮挡邮箱和用量，不要上传令牌、Cookie、API Key 或完整对话日志。

## English

AI Gauge is a free, closed-source beta for macOS 14+. Drag the universal app from the DMG into Applications. This beta is not notarized; do not disable system security. Claude, Grok and DeepSeek integrations are experimental. Credentials and local history are not included in the installer. Never attach secrets or full conversation logs to a bug report.

Build 54 estimates Codex account usage for yesterday and this month from account-reported tokens at a fixed reference rate of $1 per million tokens, using UTC dates. This is not official model pricing or an actual bill. “Yesterday tokens” uses the same day; missing data stays pending, with no local-log fallback. Hover over the estimate card for details.
