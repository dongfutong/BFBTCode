# 用手机远控 BFBT Code 终端版

Linux 上运行 `bfbtcodetui`，手机用 DTworkeasy 远控。两边使用同一套东复同账号。

## 电脑上准备

1. 安装终端版，见 [安装说明](../install/README.md)。
2. 进入要处理的文件夹，运行 `bfbtcodetui`，完成登录并设置 API Key。
3. 如果希望关机再开机后手机还能连，执行：

```
bfbtcodetui --daemon install
```

4. 生成配对链接：

```
bfbtcodetui --daemon pair
```

也可以在已经打开的 TUI 里输入 `/remote pair`。

把打印出来的 `dtworkeasy://pair?...` 链接发给手机，或在手机上扫描对应二维码。

跨账号远控时，先在主机执行 `/remote allow`，把对方账号加入白名单后再扫码。

## 手机上连接

1. 打开 DTworkeasy，用同一账号登录。
2. 进入「我的电脑」。
3. 粘贴或扫描配对链接，确认配对。
4. 点这台 Linux 设备，进入远控会话后发任务。

后台宿主在跑时，不必一直开着前台 TUI 窗口。可用 `bfbtcodetui --daemon status` 查看是否在运行。Linux 上的终端版必须处于试用或会员可用状态，过期后无法远控。

## 使用时注意

- 第一次请先在前台登录成功，再执行 `--daemon install`。没登录时启动后台会立即退出，但不会清掉已保存的登录。
- 只有 `/logout` 或 `bfbtcodetui --daemon logout` 才会退出登录。
- 手机功能菜单可将当前大模型设置保存到电脑。
- 电脑休眠、断网或服务没起来时，手机会显示设备不在线。
