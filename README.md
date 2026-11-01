# CC Control

**让 AI Passport 工牌成为 Claude / Codex 的随身遥控器。**

CC Control（电脑端名称：Codex Claude Control）配合 Windows 与 FoloToy AI Passport 使用。在工牌上查看会话状态、继续任务、发送预设、停止运行，处理已识别的审批和问题选项。

这是**公开发行仓库**，提供安装包、使用说明和版本记录。PC 核心源码不在此仓库公开；公开下载不表示软件开源。

## 下载与试玩

- [下载 Windows 版 1.0.0](https://github.com/zhh198903-ctrl/cc-control/releases/latest)
- [下载站与官方硬件购买入口](http://106.14.76.130/#cc-control-hardware)
- [在线试玩](http://106.14.76.130/cc-control-demo/)：独立的离线交互试玩固件，可实际选择会话、执行预设、审批、单选和多选、查看上下文及设置。无需蓝牙或 Wi-Fi 配网，不连接真实 AI、不控制电脑、不采集麦克风。
- [FoloToy 社区试玩](https://ai-passport.folotoy.cn/plays/community/1828/cc-control-claude-codex/)：离线交互版更新已提交，待社区审核后生效。

**正式版与试玩版分开分发。** 本仓库 Releases 中的 Windows 安装包只包含客户固件，不含离线试玩固件；自动更新也不会安装试玩版。需要遥控真实电脑时，请使用 Windows 正式版内的一键烧录。社区的离线试玩固件不能替代客户固件。

## 可以做什么

- 查看 Claude CLI、Claude 桌面 Code 会话、Codex CLI 和 Codex 桌面会话。
- 继续任务、发送常用预设、停止运行。
- 处理可识别的“允许一次 / 拒绝”审批，以及单选、分页问题和多选。
- 使用 USB 数据线、局域网、蓝牙或可选云中继。
- 通过新手指引完成连接；随包提供运行依赖、固件及安装工具，电脑无需开发环境。

操作依赖对应 AI 客户端和账号可用。桌面操作需要目标聊天可见且身份明确。自由输入、长期授权或未识别的界面请在电脑处理。

## 快速开始

1. 下载并完整解压 `CodexClaudeControl_dist_v1_0_0.zip`，运行 `CodexClaudeControl.exe`，保留同目录的 `_internal` 与 `bundled`。
2. 用 USB 数据线连接 AI Passport，在“设备”页按新手指引完成首次连接。需要安装固件时使用“一键烧录”，查看备份和保留设置提示。
3. 打开已登录的 Claude / Codex 会话，在“会话”页选择来源并连接。Codex 桌面版使用“选择桌面聊天…”；Claude CLI 需要开启对应自动续跑开关。
4. 工牌上用 UP / DOWN 选择，OK 进入或确认，长按 UP 返回。熄屏后的第一次按键只唤醒。退出电脑端使用“退出”，标题栏 X 隐藏到托盘。

无线连接和其它操作详见随包 README 与新手指引。首次体验可只用 USB，无需给工牌配网。

## 授权与范围

CC Control 为商业软件。USB、局域网、蓝牙不限次数；云中继内置 500 条消息试用，无需领取试用 Key。**CC Control 永久授权 ¥88**，不含 AI Passport 硬件与 AI 服务费用。

PC 核心采用 Cython 本机编译保护，发行包带 Ed25519 完整性校验。这能提高逆向和篡改成本，不是无法破解的加密，也不是 Windows Authenticode 签名。第三方组件遵循各自许可证，见随包许可资料。

当前发行仍有未完成的独立验收：本轮 Claude 真实账号复测、真人语音确认、人工连接切换及实际付款激活。历史版本的实测不替代这些项目。在线试玩实际运行固件交互，AI 回复为预设数据，不作为真实账号或实物验收。

可选的 `CodexClaudeControl-Skill_dist_v1_0_0.zip` 是安装和排障辅助，产品运行不依赖它。

## English

CC Control turns an AI Passport badge into a portable remote for Claude and Codex on Windows. View session status, continue a task, send a preset, stop a run, and respond to supported approvals and question cards. It supports terminal and desktop sessions through USB, LAN, Bluetooth, or an optional cloud relay.

This is a **binary distribution repository**, not the PC application's source repository. Download and extract the complete Windows package, run `CodexClaudeControl.exe`, connect the badge by USB, then follow onboarding to connect your AI session.

USB, LAN, and Bluetooth are unmetered. The cloud relay includes a 500-message trial. **CC Control lifetime license ¥88**, excluding hardware and AI service fees. Third-party licenses remain applicable. The interactive trial runs separate offline firmware with scripted data, actual buttons, session actions, approvals, and question flows. Bluetooth, Wi-Fi, and microphone capture are disabled. It does not control your PC. Windows Releases and the stable update feed contain only customer firmware, never the trial firmware. The community trial update is pending review.

See [CHANGELOG.md](CHANGELOG.md) and [Releases](https://github.com/zhh198903-ctrl/cc-control/releases).
