# 0.1.0 Beta · build 54 — 2026-09-07

- Codex 昨日／当月金额改为账户已报 Token × $1 / 百万 Token 的统一参考估算，不再使用本机费用；非模型官方报价或实际账单。
- “今日 Token”改为“昨日 Token”，与“本账户昨日估算”按同一 UTC 日期读取，缺失数据保留“待更新”。
- 金额卡片移除两行常驻说明，折算口径改为悬停提示；中英文标签同步更新。
- 收紧账户身份匹配，身份未知或不一致时不展示账户估算。
- 中英文 README 更新统计口径、昨日数据说明及微信咖啡赞赏码；宣传图片保持原样。

- Codex estimates now use account-reported tokens at a fixed $1 per million token benchmark, not local costs, official model pricing, or an actual bill.
- Show yesterday's tokens and estimate for the same UTC day; missing data remains pending.
- Move calculation notes to hover help and update Chinese and English labels.
- Hide account analytics when account identity is unknown or mismatched.
- Update both READMEs, including optional WeChat coffee support. Promotional images are unchanged.

This beta remains ad-hoc signed and not notarized. New-device and cross-device account validation remain pending.

# 0.1.0 Beta · build 53 — 2026-09-07

- 设置旁新增单色／彩色快捷切换，支持中英文提示。
- 柱状图悬停时在下方显示日期与精确 Token 数，移开隐藏，行高固定。
- 修复英文圆环标签重叠与 100% 截断。
- 修复重置时间区域切换语言后未及时刷新的问题。

- Added a color/monochrome toggle beside Settings.
- Show exact daily token usage below the chart on hover, without layout jumps.
- Fixed English quota-label overlap and 100% truncation.
- Fixed reset-time labels not updating when switching languages.

This beta is ad-hoc signed and not notarized. Existing device/account validation limits remain.

# 0.1.0 Beta — 2026-09-07

- 增加隐私、使用许可及第三方材料入口。
- DeepSeek 登录窗口限制为官方平台顶层页面，外部主动链接交给浏览器。
- Claude/Grok/DeepSeek 菜单标注实验性。
- 保留全部原有白噪音与音频素材；完善许可说明，不分发未启用的 WorkBuddy 图标。
- 完整安装包与版本核验、SHA-256 校验及公开发布检查流程。

待验收：Developer ID 签名和 Apple 公证、Intel/macOS 14 实机安装、实验性供应商的真实账号流程。当前包不得标为已公证正式版。
