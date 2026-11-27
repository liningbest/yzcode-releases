<h1 align="center">YZ Code</h1>

<p align="center">
  <strong>Multi-Agent AI Coding Desktop Workbench · 多智能体 AI 编程桌面工作台</strong>
</p>

<p align="center">
  <a href="#english">English</a> · <a href="#简体中文">简体中文</a> · <a href="https://github.com/liningbest/yzcode-releases/releases/latest">Latest Release / 下载最新版</a> · <a href="https://github.com/liningbest/yzcode-releases/issues">Issues / 问题反馈</a>
</p>

---

<a id="english"></a>

## English

**YZ Code** is a lightweight, high-performance desktop workbench for coding agents. Connect your own subscriptions across **Claude Code, Codex, Cursor, Antigravity, OpenCode, Grok, Kiro, and Pi** in one unified interface.

### Highlights
- **Zero Telemetry & Local-First Privacy**: All third-party analytics and telemetry endpoints are permanently disabled. Conversations and code stay on your own machine.
- **Bilingual UI (Chinese & English)**: Clean Chinese and English interface out of the box for macOS (Apple Silicon) and Windows (x64).
- **Multi-Agent & Worktree Isolation**: Run parallel sessions across Git worktrees, inspect diffs, test web apps in the built-in preview browser, and drive iOS/Android simulators.
- **Plugin Center & Cross-Engine Skill Sync**: Built-in starter engineering plugins, one-click Skill sync across Codex / OpenCode / Claude Code / Cursor / Antigravity, plus exportable team presets.
- **Real-Time Team Webhooks**: Native Feishu (Lark), DingTalk, and WeCom notifications when turns finish, need approval, or fail.
- **Compliant Antigravity Quota Sync**: Uses Antigravity CLI's official `statusLine` hook (`stack_with_default: true`) to display remaining quota in **Usage → Limits** without touching OAuth tokens or private APIs.
- **Automatic In-App Update Reminders**: Checks for updates every 30 minutes and prompts with one-click download and restart-to-install.

### Download

Visit **[Latest Release](https://github.com/liningbest/yzcode-releases/releases/latest)** to download the installer for your platform:

| Platform | Asset | Notes |
| --- | --- | --- |
| **macOS (Apple Silicon / M1–M4)** | `YZ-Code-<version>-arm64.dmg` | Drag `YZ Code.app` into `/Applications` |
| **Windows (x64)** | `YZ-Code-<version>-x64.exe` | Run installer; supports automatic in-app updates |

> Once installed, future releases are delivered automatically via in-app update reminders.

### First-Launch Notes (Unsigned Builds)

Free community builds are currently distributed without commercial Apple Developer / Windows Authenticode certificates, so your OS may show a security prompt on the first launch:

- **macOS**: If macOS says the app is *"damaged"* or *"cannot be verified"*, drag `YZ Code.app` into `/Applications` and run once in Terminal:
  ```bash
  xattr -cr "/Applications/YZ Code.app"
  ```
  Subsequent in-app updates automatically clear the quarantine flag.
- **Windows**: If Windows Defender SmartScreen appears, click **More info** → **Run anyway**.

### Feedback & Support

Please report bugs or request features in **[GitHub Issues](https://github.com/liningbest/yzcode-releases/issues)** (include your OS and YZ Code version).

### Privacy & Open-Source Notice

- **Privacy**: Telemetry is permanently disabled. YZ Code does not collect or transmit your source code, prompts, or usage analytics. Model requests go directly to the providers you configure and sign in to.
- **License & Attribution**: An unofficial derivative build based on the MIT-licensed [T3 Code](https://github.com/pingdotgg/t3code) source code. YZ Code is an independent project and is **not** affiliated with, endorsed by, or maintained by T3 Tools, Inc. See [LICENSE](./LICENSE) (and **Settings → About → Open source licenses** inside the app) for full MIT copyright and license notices.

---

<a id="简体中文"></a>

## 简体中文

**YZ Code** 是一款轻量、高性能的多智能体 AI 编程桌面工作台，统一接入 **Claude Code、Codex、Cursor、Antigravity、OpenCode、Grok、Kiro、Pi** 等本地编程智能体（自带账号 / 订阅即可使用）。

### 核心特性
- **永久零遥测与本地隐私优先**：彻底禁用所有第三方埋点与遥测上报，代码与对话数据完全留在你自己的设备上。
- **开箱即用中英文界面**：支持简体中文与英文自由切换，适配 macOS（Apple Silicon）与 Windows（x64）。
- **多智能体与多工作区并行**：支持 Git Worktree 隔离、多会话并行、内置预览浏览器测试与移动设备模拟器联调。
- **插件中心与跨引擎 Skill 同步**：内置常用研发规范插件，一键同步 Skills 到 Codex / OpenCode / Claude Code / Cursor / Antigravity，支持团队预设导入导出。
- **群机器人实时通知**：内置飞书、钉钉、企业微信 Webhook 通知，任务完成、等待审批或异常时即时提醒。
- **Antigravity 合规配额同步**：基于 Antigravity CLI 官方 `statusLine` 回调机制（保留原生状态栏），在「用量 → 限制」中安全查看剩余配额，不触碰 OAuth Token、不请求任何私有接口。
- **应用内自动更新提醒**：客户端每 30 分钟静默检查更新，发现新版本自动弹窗提示一键下载与重启安装。

### 立即下载

前往 **[Latest Release（最新版本）](https://github.com/liningbest/yzcode-releases/releases/latest)** 下载对应平台安装包：

| 平台 | 文件 | 说明 |
| --- | --- | --- |
| **macOS (Apple Silicon / M1–M4)** | `YZ-Code-<version>-arm64.dmg` | 下载后拖入「应用程序」文件夹 |
| **Windows (x64)** | `YZ-Code-<version>-x64.exe` | 双击安装，支持应用内自动增量更新 |

> 安装完成后，客户端会自动检测并提示后续版本更新，无需每次手动来仓库下载。

### 首次安装提示（未签名安装包说明）

目前免费分发版本尚未购买 Apple Developer / Windows 商业代码签名证书，首次安装打开时系统会弹出安全拦截提示，按以下步骤放行一次即可：

- **macOS**：若提示 **「已损坏，无法打开」** 或 **「无法验证开发者」**，将 `YZ Code.app` 拖入 `/Applications` 后，在终端执行一次：
  ```bash
  xattr -cr "/Applications/YZ Code.app"
  ```
  后续应用内自动更新会自动清除隔离属性，无需再次执行。
- **Windows**：若出现 **Windows Defender SmartScreen「Windows 已保护你的电脑」** 提示，点击 **「更多信息」→「仍要运行」** 即可安装。

### 问题反馈与建议

欢迎在 **[GitHub Issues](https://github.com/liningbest/yzcode-releases/issues)** 提交 Bug 报告或功能建议（请附带系统版本与 YZ Code 版本号）。

### 隐私与开源合规声明

- **隐私声明**：YZ Code 已永久禁用遥测统计，不会收集或上报你的代码、对话内容、使用习惯或设备信息。使用各 AI 智能体时，请求仅直接发送至你自行配置与登录的模型服务商。
- **开源协议与非官方声明**：YZ Code 是基于开源项目 [T3 Code](https://github.com/pingdotgg/t3code)（MIT 协议）源代码构建的**非官方独立定制版本**，与 T3 Tools, Inc. 无任何官方关联、背书或赞助关系。完整 MIT 许可与版权声明见本仓库根目录的 [LICENSE](./LICENSE) 文件，也可在客户端 **设置 → 关于 → 开源许可** 中查看。
