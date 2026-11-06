# 安装说明

**BFBT Code** 是东复同科技的 AI 编程助手（AI coding agent / coding assistant）。官网账号同时用于 BFBT Code 和 DTworkeasy，只需注册一次。打开官网「下载中心」或本仓库 [GitHub Releases](https://github.com/dongfutong/BFBTCode/releases)，按设备选择软件。

官网文档：<https://www.dtrony.com/docs/installation> · <https://www.dtrony.com/docs/install-tui>

## 支持的安装包

| 系统 | 软件 | 常见文件 | 说明 |
|---|---|---|---|
| Windows 10/11 64 位 | BFBT Code 桌面版 | `.msi` | 试用或会员可用 |
| macOS 11+ Apple Silicon | BFBT Code 桌面版 | `.dmg` | 试用或会员可用；Intel Mac 暂未提供 |
| Linux x86_64 | BFBT Code 终端版（TUI） | `.tar.gz` 或一行脚本 | 试用或会员可用；不需要 Rust，也不需要源码 |
| Android | DTworkeasy | `.apk` | 注册即可免费使用 |
| iOS | DTworkeasy | App Store | 注册即可免费使用 |

当前 Release 中实际提供的文件名以下载页面为准。最新桌面版 / TUI 见 [`v1.0.8.26102008`](https://github.com/dongfutong/BFBTCode/releases/tag/v1.0.8.26102008)。

## Windows

1. 从 [Releases](https://github.com/dongfutong/BFBTCode/releases) 或官网下载中心保存最新 `.msi`（当前示例：`BFBTcode_1.0.8.26102008_x64_en-US.msi`）。
2. 双击安装包，按提示完成安装。
3. 打开「开始」菜单，搜索 **BFBTcode** 并打开。
4. 选择一个工作文件夹。

如果出现「Windows 已保护你的电脑」，先确认安装包来自本仓库 Release 或官网，再点「更多信息」→「仍要运行」。不要从压缩包预览窗口直接运行。

卸载：Windows 设置 → 应用 → 搜索 BFBTcode → 卸载。

## macOS（Apple Silicon）

桌面版当前仅发布 Apple Silicon（aarch64）DMG；Intel 机型暂未提供。支持 macOS 11 (Big Sur) 及以上。官网说明：<https://www.dtrony.com/docs/installation>

1. 从 [Releases](https://github.com/dongfutong/BFBTCode/releases) 或官网下载中心保存最新 `.dmg`（当前示例：`BFBTcode_1.0.8.26102009_aarch64.dmg`）。
2. 双击打开 `.dmg`，把 **BFBTcode** 拖进「应用程序」。不要直接在 dmg 窗口中长期运行。
3. 第一次打开时若提示「无法打开，因为它来自身份不明的开发者」，打开「系统设置」→「隐私与安全性」，点底部「仍要打开」。
4. 打开应用，登录东复同账号，选择工作文件夹。

卸载：在「应用程序」文件夹把 BFBTcode 移到废纸篓。

## Linux（终端版）

建议 Ubuntu 22.04 及以上，x86_64。不需要安装 Rust，也不需要下载源码。

在终端执行：

```
curl -fsSL 'https://www.dtrony.com/install-tui.sh' | sudo sh
```

同一条命令也可以用来升级。也可以直接下载 `bfbtcodetui-linux-x86_64.tar.gz` 后按包内说明安装。

启动：

```
bfbtcodetui
```

按提示用东复同账号登录。输入问题后按 Enter 发送；输入 `/help` 查看命令；空闲时按 Ctrl+C 退出。建议先进入你要处理的文件夹，再启动程序。

如果要用手机远控这台 Linux 电脑，建议装好后开启开机自启：

1. 先在前台运行一次 `bfbtcodetui`，完成登录并设置 API Key。
2. 再执行 `bfbtcodetui --daemon install`。

常用命令：

```
bfbtcodetui --daemon status
bfbtcodetui --daemon pair
bfbtcodetui --daemon uninstall
```

登录保存在本机，重启不会退出。只有在 TUI 里输入 `/logout`，或执行 `bfbtcodetui --daemon logout`，才会退出登录。

## Android（DTworkeasy）

1. 从官网下载中心或 [DTworkeasy-Mobile Releases](https://github.com/dongfutong/DTworkeasy-Mobile/releases) 下载 APK。
2. 打开下载的 APK。
3. 如系统提示未知来源，允许当前浏览器或文件管理器安装应用。
4. 打开 DTworkeasy，使用东复同账号登录。

请只从官网或官方仓库 Release 下载 APK。

## iOS（DTworkeasy）

iPhone 或 iPad 请在 App Store 安装 DTworkeasy，并用同一套官网账号登录。

官方商店：<https://apps.apple.com/cn/app/dtworkeasy/id6806894230>

也可在官网下载中心选择 iOS，点击「前往 App Store」。

安装完成后请继续阅读 [登录说明](../login/README.md)。BFBT Code 桌面版和终端版需要试用或会员有效期内才能使用。
