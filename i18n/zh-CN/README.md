# BFBT Code — AI 编程助手 / AI coding agent

**BFBT Code**（亦称 BFBTCode）是东复同科技推出的 AI 编程助手（AI coding agent / coding assistant），面向写代码、学习和日常工作。桌面版支持 **Windows** 与 **macOS（Apple Silicon）**，另有 **Linux** 终端版（TUI）。可用手机上的 DTworkeasy 远控电脑里的 BFBT Code。

本仓库只提供安装包和用户文档，不包含源代码。

| | |
|---|---|
| 官网 | <https://www.dtrony.com> |
| 文档中心 | <https://www.dtrony.com/docs> |
| 下载 | [GitHub Releases](https://github.com/dongfutong/BFBTCode/releases) |
| 会员 | [会员权益](../../docs/token/README.md) |

## 下载与安装

从 [GitHub Releases](https://github.com/dongfutong/BFBTCode/releases) 或官网下载中心获取与系统匹配的安装包，按 [安装说明](../../docs/install/README.md) 完成安装。不要下载或编译源码。

- Windows 10/11 64 位：BFBT Code 桌面版（`.msi`）
- macOS 11+ Apple Silicon：BFBT Code 桌面版（`.dmg`）；Intel Mac 暂未提供
- Linux x86_64：BFBT Code 终端版（`bfbtcodetui`）
- Android：DTworkeasy（注册即可免费使用）
- iOS：DTworkeasy（[App Store](https://apps.apple.com/cn/app/dtworkeasy/id6806894230)）

Linux 也可执行：`curl -fsSL 'https://www.dtrony.com/install-tui.sh' | sudo sh`

## 登录与使用

启动软件，用东复同官网账号登录。桌面版选择工作目录后，在设置中填写 API Key，发送「你好」。终端版按提示登录并设置 API Key，输入 `/help` 查看命令。

## Desktop 设置

在「设置」中配置语言、账号、模型服务、API Key、工作目录、远程连接和权限。当前支持 14 种界面语言。API Key、密码和 Token 不得上传到仓库或 Issue。

## 会员

BFBT Code 和 BFBTbridge 需要试用或会员有效期内才能使用；新用户注册后自动开通 90 天试用。DTworkeasy 注册即可免费使用。会员费不含大模型 Token。详见 [会员权益](../../docs/token/README.md)。

问题请提交 [GitHub Issue](https://github.com/dongfutong/BFBTCode/issues) 或 [Gitee Issue](https://gitee.com/dongfutong2026/bfbtcode/issues)，并删除所有敏感信息。也可使用官网「意见反馈」。
