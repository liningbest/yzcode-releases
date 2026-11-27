# YZ Code

**YZ Code** 是一款轻量、高性能的多智能体 AI 编程桌面工作台，统一接入 **Claude Code、Codex、Cursor、Antigravity、OpenCode、Grok、Kiro、Pi** 等本地编程智能体（Bring Your Own Subscription）。

- **永久零遥测与本地隐私优先**：彻底禁用所有第三方埋点与遥测上报，对话与数据完全留在你自己的设备上。
- **开箱即用简体中文界面**：支持中英文自由切换，适配 macOS（Apple Silicon）与 Windows（x64）。
- **多智能体与多工作区并行**：支持 Git Worktree 隔离、多会话并行、内置预览浏览器测试与移动设备模拟器联调。
- **插件中心与跨引擎 Skill 同步**：内置常用研发规范插件，一键同步 Skills 到 Codex / OpenCode / Claude Code / Cursor / Antigravity，支持团队预设导入导出。
- **群机器人实时通知**：内置飞书、钉钉、企业微信 Webhook 通知，任务完成、等待审批或异常时即时提醒。
- **Antigravity 合规配额同步**：基于 Antigravity CLI 官方 `statusLine` 回调机制，在「用量 → 限制」中安全查看剩余配额。
- **应用内自动更新提醒**：客户端每 30 分钟静默检查更新，发现新版本自动弹窗提示一键下载与重启安装。

---

## 立即下载

前往 **[Latest Release（最新版本）](https://github.com/liningbest/yzcode-releases/releases/latest)** 下载对应平台安装包：

| 平台 | 文件 | 说明 |
| --- | --- | --- |
| **macOS (Apple Silicon / M1–M4)** | `YZ-Code-<version>-arm64.dmg` | 下载后拖入「应用程序」文件夹 |
| **Windows (x64)** | `YZ-Code-<version>-x64.exe` | 双击安装，支持应用内自动增量更新 |

> 安装完成后，客户端会自动检测并提示后续版本更新，无需每次手动来仓库下载。

---

## 首次安装提示（未签名安装包说明）

目前免费分发版本尚未购买 Apple Developer / Windows 商业代码签名证书，**首次安装打开时系统会弹出安全拦截提示**，属于正常现象，按以下步骤放行一次即可：

### macOS
若提示 **「已损坏，无法打开」** 或 **「无法验证开发者」**，将 `YZ Code.app` 拖入 `/Applications` 后，打开终端执行一次：

```bash
xattr -cr "/Applications/YZ Code.app"
```

执行后即可正常双击打开，后续应用内自动更新会自动清除隔离属性，无需再次执行。

### Windows
若出现 **Windows Defender SmartScreen「Windows 已保护你的电脑」** 蓝屏提示：
1. 点击提示文字中的 **「更多信息」**（More info）
2. 点击下方出现的 **「仍要运行」**（Run anyway）即可开始安装。

---

## 问题反馈与建议

欢迎在 **[GitHub Issues](https://github.com/liningbest/yzcode-releases/issues)** 提交 Bug 报告或功能建议（请附带系统版本与 YZ Code 版本号）。

---

## 隐私与开源合规声明

- **隐私声明**：YZ Code 已永久禁用遥测统计，不会收集或上报你的代码、对话内容、使用习惯或设备信息。使用各 AI 智能体时，请求仅直接发送至你自行配置与登录的模型服务商。
- **开源协议与非官方声明**：YZ Code 是基于开源项目 [T3 Code](https://github.com/pingdotgg/t3code)（MIT 协议）源代码构建的**非官方独立定制版本**，与 T3 Tools, Inc. 无任何官方关联、背书或赞助关系。
- 完整 MIT 许可与版权声明见本仓库根目录的 [LICENSE](./LICENSE) 文件，同时也可在客户端 **设置 → 关于 → 开源许可** 中查看。

> An unofficial derivative build based on the MIT-licensed [T3 Code](https://github.com/pingdotgg/t3code) source code. YZ Code is an independent project and is not affiliated with, endorsed by, or maintained by T3 Tools, Inc.
