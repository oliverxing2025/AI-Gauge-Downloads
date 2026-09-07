# 发布状态 / Release status

当前为 Beta 测试包，不是已公证正式发行版。

当前版本：0.1.0 Beta · build 54。新增账户统一参考金额估算、UTC 昨日 Token 与昨日估算。计算测试覆盖缺失与零值、跨设备同数据一致性、跨月／跨年／闰日及 UTC 边界；实际跨设备账户验收仍待完成。

已落实：凭据隐私说明、闭源免费使用许可与第三方许可区分、登录顶层域名限制、实验性标识、音频原样保留与许可记录、DMG 版本/主程序一致性检查、下载文件白名单与 SHA-256、本地凭据特征扫描脚本、GitHub 两项保护状态只读检查。

外部前置条件：本机没有 Developer ID Application 证书；Apple Development 证书不适用于此分发流程。需有效 Developer ID 签名身份及存于钥匙串的 notarytool profile，才可执行 scripts/sign-and-notarize.sh。该脚本尚未用真实证书完成端到端验证。

真实账号及设备验收：Claude/Grok/DeepSeek 完整登录链路、Intel Mac、macOS 14、全新用户首次启动、钥匙串拒绝后重试及换账号，仍需测试者确认。不能以模拟测试替代这些验收。

音频：按用户要求全部保留。雨声及机舱素材的上游 CC0 声明已记录，原始授权尚待核实；不把这项标为已完成。
