# 第一次使用

**BFBT Code** 是用于写代码、学习和日常工作的 AI 编程助手。安装完成后，先登录东复同账号，再设置大模型 API Key。没有 API Key，软件无法回复。

API Key 相当于密码，不要发给别人，也不要贴到聊天或截图里。

官网说明：<https://www.dtrony.com/docs/updates>

## 桌面版（Windows / macOS）

1. 打开 BFBTcode，选择工作文件夹。
2. 打开右侧「设置」。
3. 选择模型服务商，粘贴 API Key，保存。
4. 在输入框发送「你好」。

能收到回复，说明设置成功。macOS 为 Apple Silicon 桌面版；Intel Mac 暂未提供。

## 终端版（Linux）

第一次启动会提示输入 API Key。以后更换可输入：

```
/api set deepseek sk-...
```

把 `sk-...` 换成自己的 Key。其他厂商把 `deepseek` 换成 `openai`、`glm`、`minimax`、`qwen` 或 `moonshot`。

输入 `/model` 可切换模型，输入 `/help` 查看全部命令。

## DTworkeasy

打开应用后，用官网同一套账号登录即可。主题卡片和节点列表的 AI 对已登录用户开放。Android 从官网或官方仓库安装；iOS 从 [App Store](https://apps.apple.com/cn/app/dtworkeasy/id6806894230) 安装。

## 常用操作

- 新建会话：为不同任务建立独立上下文。
- 恢复会话：继续之前的工作。
- 附加文件：只选择完成任务所需的文件，避免上传敏感信息。
- 中止任务：任务运行期间使用停止按钮。
- 手机远控：见 [远控桌面版](../remote/desktop.md) 和 [远控终端版](../remote/tui.md)。

BFBT Code 可能读取、修改项目文件或执行工具操作。请先备份重要文件，并审查模型输出。BFBT Code 需要试用或会员；会员费不含大模型 Token。
