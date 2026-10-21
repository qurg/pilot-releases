# Pilot 客户端下载

Pilot 是在电脑上跑的 AI 工作助理：能执行命令、读写本机文件，通过 skill 接入各种工具，默认连 Router（https://api.szcvip.com）。

## 下载

| 系统 | 下载（始终是最新版） |
|---|---|
| Windows 10 / 11（x64） | [Pilot-win.zip](https://github.com/qurg/pilot-releases/releases/latest/download/Pilot-win.zip) |
| macOS 14 及以上（Apple 芯片 M1 及以后） | [Pilot-mac.zip](https://github.com/qurg/pilot-releases/releases/latest/download/Pilot-mac.zip) |

历史版本见 [Releases](https://github.com/qurg/pilot-releases/releases)。

## Windows：三步用起来

1. 右键 zip →「属性」→ 勾选「解除锁定」→ 确定，解压到任意目录，双击 `Pilot.exe`。（提示「Windows 已保护你的电脑」时点「更多信息 → 仍要运行」。）
2. 打开 [Router 令牌页](https://api.szcvip.com/console/token)，新建一个令牌，在那一行点「聊天 → Pilot」，浏览器问是否打开时选「打开」：服务地址和 Key 自动填好。
3. Pilot 里打开「设置」，点「从服务获取」拿模型列表，留下要用的几个（第一行是默认），保存。

升级：下载新版解压覆盖原目录即可，对话和设置在 `%APPDATA%\Pilot\`，不会丢。

## Mac：三步用起来

1. 解压后把 `Pilot.app` 拖进「应用程序」。第一次打开会提示「无法验证开发者」：到「系统设置 → 隐私与安全性」最下面点「仍要打开」。也可以在终端执行一次 `xattr -dr com.apple.quarantine /Applications/Pilot.app` 再打开。
2. 打开 [Router 令牌页](https://api.szcvip.com/console/token) 新建一个令牌，复制 Key。
3. Pilot 的「设置 → 模型」里添加服务商，类型选「OpenAI 兼容」，Base URL 填 `https://api.szcvip.com/v1`，粘贴 Key；再添加要用的模型名（和 Router「模型广场」里的名字一致），点「测试」确认能连通，保存。

升级：下载新版替换「应用程序」里的 Pilot.app，对话和设置在 `~/Library/Application Support/Pilot/`，不会丢。

这里只放安装包，不含源码。
