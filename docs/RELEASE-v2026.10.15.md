# Gemini Relay 2026.10.15 · macOS 分享版 / Community Build

[中文说明](https://github.com/TGmszrcsz/gemini-relay#readme) · [English guide](https://github.com/TGmszrcsz/gemini-relay/blob/main/README.en.md)

[![Telegram @mszrcsz](https://raw.githubusercontent.com/TGmszrcsz/gemini-relay/main/assets/telegram.svg)](https://t.me/mszrcsz)
[![Donate · NOWPayments](https://raw.githubusercontent.com/TGmszrcsz/gemini-relay/main/assets/donate.svg)](https://nowpayments.io/embeds/donation-widget?api_key=0a09a5b0-4590-4b3f-a3cf-c4fa08d67ada)

## 中文

通过自己的 API URL 与 API Key 使用 Gemini macOS 客户端，无需 Google 账号，并加入基础项目编程、代码编辑、交互预览与 MCP 连接。

### 本版功能

- 验证 API 连接并查看可用模型，在对话中切换模型。
- 流式对话、执行状态与耗时、本地历史和持久删除。
- 在对话区域创建或打开项目，拖入文件及文件夹。
- 读取、修改项目代码，运行命令与测试；代码窗口支持编辑、保存、自动刷新和冲突提示。
- HTML/SVG 内容与 HTML 交互预览。
- MCP stdio 与 Streamable HTTP，支持工具发现与调用。
- 新增界面跟随系统语言，保留 Telegram 鸣谢与捐赠入口。

### 下载与使用

下载下方 Assets 中的 **`Gemini-Relay-2026.10.15-arm64.dmg`**，打开后拖到 Applications。仅支持 **Apple Silicon，macOS 15+**。普通聊天无需安装 Node.js。

首次打开的 API 字段为空，请填写自己的地址与密钥。服务需支持 Gemini 原生 `/v1beta/models/...:streamGenerateContent` 以及 `/v1/models`。安装包不带打包者的 API、聊天、项目或 MCP 配置。

本包采用 ad-hoc 签名，未进行 Apple Developer ID 签名或公证。如果 macOS 阻止打开，确认来源后在“系统设置 → 隐私与安全性”选择“仍要打开”。

### 边界与验证

这是基于原有 Gemini 客户端加入 API 适配与 AppKit 功能的修改版本，独立于 Google，面向基础 Vibe Coding。图片和视频生成不可用；命令限时约 50 秒，编辑器支持最大 2 MB 的 UTF-8 文件。MCP OAuth、旧版独立 SSE 和 prompts/resources 浏览暂未实现。

已验证空配置首次启动、安装包完整性与签名、个人数据排除、实际项目代码修改和测试、编辑刷新与冲突，以及 MCP stdio/HTTP 协议往返。模型触发 MCP 的完整端到端验证尚未完成。

## English

Use the Gemini macOS client with your own API URL and key, without a Google account. This build adds basic project coding, a code editor, interactive previews and MCP connections.

### Included

- Verify your API connection, discover available models and select a model in chat.
- Streamed conversations, activity and elapsed time, local history and persistent deletion.
- Create or open projects from chat and drop files or folders as references.
- Read and change code, run commands and tests, and edit files in a code window with saving, automatic refresh and conflict handling.
- HTML/SVG content and interactive HTML previews.
- MCP over stdio and Streamable HTTP, with tool discovery and calls.
- Added interfaces follow the system language; Telegram thanks and donation links remain available.

### Download and setup

Download **`Gemini-Relay-2026.10.15-arm64.dmg`** from Assets and drag the app to Applications. Requires **Apple Silicon and macOS 15+**. Chat needs no Node.js.

The first-run URL and key fields are empty. Enter your own credentials for a provider supporting `/v1beta/models/...:streamGenerateContent` and `/v1/models`. The installer includes none of the packager's API settings, chats, projects or MCP configuration.

This build is ad-hoc signed, without Apple Developer ID signing or notarization. If macOS blocks it, verify the source and use System Settings → Privacy & Security → Open Anyway.

### Scope and validation

This is a modified original Gemini client with an API adapter and AppKit additions, independent of Google. It focuses on basic Vibe Coding. Image/video generation is unavailable. Commands have an approximately 50-second limit; the editor supports UTF-8 files up to 2 MB. MCP OAuth, legacy standalone SSE and prompts/resources browsing are not implemented.

Validated: clean first launch, installer integrity and signature, exclusion of personal data, real project code changes and tests, editor refresh and conflicts, and MCP stdio/HTTP protocol round trips. Full model-to-MCP end-to-end verification has not been completed.

## Screenshots / 功能截图

Actual app screenshots, cropped or redacted to remove personal information. / 真实应用截图，已裁切或遮盖个人信息。

![API connection / API 连接](https://raw.githubusercontent.com/TGmszrcsz/gemini-relay/main/assets/screenshots/api-connection-en.png)

![Project code and test / 项目代码与测试](https://raw.githubusercontent.com/TGmszrcsz/gemini-relay/main/assets/screenshots/project-code-test.png)

![HTML live preview / HTML 实时预览](https://raw.githubusercontent.com/TGmszrcsz/gemini-relay/main/assets/screenshots/html-live-preview.png)

## SHA-256

```text
b64b6d8bb1230c19b015a13009dfeb252cf163340137d2b2513f9a89f44aeeb1  Gemini-Relay-2026.10.15-arm64.dmg
```

特别鸣谢 / Special thanks: **[Telegram @mszrcsz](https://t.me/mszrcsz)** · **[捐赠 / Donate](https://nowpayments.io/embeds/donation-widget?api_key=0a09a5b0-4590-4b3f-a3cf-c4fa08d67ada)**
