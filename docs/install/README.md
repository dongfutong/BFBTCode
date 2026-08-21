# 安装说明

官网账号同时用于 BFBT Code 和 DTworkeasy，只需注册一次。打开官网「下载中心」或本仓库 [Releases](../../../releases)，按设备选择软件。

## 支持的安装包

| 系统 | 软件 | 常见文件 | 说明 |
|---|---|---|---|
| Windows 10/11 64 位 | BFBT Code 桌面版 | `.msi` | 试用或会员可用 |
| Linux x86_64 | BFBT Code 终端版（TUI） | `.tar.gz` | 试用或会员可用；不需要 Rust，也不需要源码 |
| Android | DTworkeasy | `.apk` | 注册即可免费使用 |
| macOS | BFBT Code 桌面版 | — | 暂未上架 |
| iOS | DTworkeasy | — | 暂未上架 |

当前 Release 中实际提供的文件名以下载页面为准。

## Windows

1. 下载 `BFBTcode_1.0.0_x64_en-US.msi`。
2. 双击安装包，按提示完成安装。
3. 打开「开始」菜单，搜索 **BFBTcode** 并打开。
4. 选择一个工作文件夹。

如果出现「Windows 已保护你的电脑」，先确认安装包来自本仓库 Release 或官网，再点「更多信息」→「仍要运行」。不要从压缩包预览窗口直接运行。

卸载：Windows 设置 → 应用 → 搜索 BFBTcode → 卸载。

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

1. 下载 `DTworkeasy-1.0.6.apk`。
2. 打开下载的 APK。
3. 如系统提示未知来源，允许当前浏览器或文件管理器安装应用。
4. 打开 DTworkeasy，使用东复同账号登录。

请只从官网或本仓库 Release 下载 APK。

## macOS / iOS

macOS 桌面版和 DTworkeasy iOS 版暂未上架，敬请期待。

安装完成后请继续阅读 [登录说明](../login/README.md)。
