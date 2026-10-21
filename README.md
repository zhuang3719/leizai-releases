# 雷仔（Leizai）

> **你的电脑里，住着一支 AI 团队。**
> 一支本地运行、各司其职、还会越用越懂你的 AI 团队。你说人话，它拆活、分工、干活——数据一步都不出本机。

<p align="center">
  <a href="https://leizai.cc/download.html"><b>⬇️ 下载桌面版</b></a> &nbsp;|&nbsp;
  <a href="https://leizai.cc"><b>🌐 访问官网</b></a> &nbsp;|&nbsp;
  <a href="https://leizai.cc/docs.html">文档</a> &nbsp;|&nbsp;
  <a href="https://leizai.cc/pricing.html">定价</a> &nbsp;|&nbsp;
  <a href="https://leizai.cc/opensource.html">开源说明</a>
</p>

<p align="center"><b>当前版本：v0.1.24</b></p>

---

## 这是什么

雷仔是一支跑在**你自己电脑上**的 AI 团队：一个负责决策与拆解的「主我」，加一队各管一摊的「雷影」（写代码、做界面、写文案、跑测试、查资料、谈客户）。

- **开发者 / 一人公司**：需求写完没人帮你测，代码改到凌晨还怕漏 bug。
- **律师、会计这类碰数据的**：想把合同、账目交给 AI，又不敢传上去。
- **不太会用 AI 的老板**：别人说 AI 能干活，你打开对话框却不知道从哪问起。

说清楚要什么，剩下的它来。

---

## 凭啥用它

**🔒 数据不出本机**
文件、聊天、成果全部写在你本机磁盘；除了调用你自己配置的模型服务，不上传、不入第三方。

**🧠 聊再久，也不会忘事**
对话长成一棵「会话树」：主干是主线，按主题分出枝干。旧内容自动收起来，需要时顺着枝、搜个词就翻得回来——一个会话走完一个项目，不用开一堆会话。

**👥 一队雷影替你干活**
主我拆解派活，专长雷影并行执行、自动接力；进度、决定、产出都留档可查。

**💰 同样的活，花得更少**
我们针对 DeepSeek 的缓存命中做了深层次优化——同样的活，消耗只有同类助手的一小部分。

> 另有 **Pro**（更高协作规模 / 企业能力，**仍在本机运行**），详见[官网](https://leizai.cc)。

---

## 界面截图

> 截图占位（客户端界面）—— 随仓上传时替换为真实截图。

![雷仔客户端 · 项目视图](docs/assets/app-projects.png)
![雷仔客户端 · 多雷影协作](docs/assets/app-conversation.png)

---

## 快速上手

1. **下载**：到[官网下载页](https://leizai.cc/download.html)取 Windows 桌面版（Setup）或免安装便携版（Portable）。
2. **安装**：运行安装包，所有数据默认写入本机。
3. **接模型**：在「设置」里填入你自己申请的模型 API Key，选择模型。
4. **开工**：新建一个会话，直接说要什么即可。

> ⚠️ 请勿把真实密钥写进会被提交的文件；密钥只填在你本机的软件设置里。

---

## 下载桌面版

**<https://leizai.cc/download.html>**

- Windows 桌面版（Setup）与免安装便携版（Portable）
- 下载后请核对页面上的 **SHA-256** 校验值
- 免费版 **Lite** 即可上手；更高协作规模可选 **Pro**

---

## 数据位置与卸载（桌面版）

- **数据根**：`%LOCALAPPDATA%\LeiZaiData`（含 `config*.json`、`data/`、`workspace/`、`projects/`、`logs/`）。
- **卸载不会删除数据**：卸载程序只移除安装目录 `%LOCALAPPDATA%\LeiZai`（程序文件），数据目录独立存放，重装后原数据仍在。
- **手动清理**：如需彻底清除，关闭程序后删除 `%LOCALAPPDATA%\LeiZaiData` 即可。
- 便携版（Portable）数据跟随解压目录；可用 `portable.flag` 标记绿色目录。

---

## 开源范围与许可

- **引擎与外壳开源**：基础引擎、桌面外壳、协议与界面以 **Apache License 2.0** 发布，可审查、可自行部署。详见 [LICENSE](https://github.com/zhuang3719/leizai-agent/blob/master/LICENSE)。
- **核心能力闭源**：会话树、雷影、记忆、进化、反思、信箱等核心能力为闭源模块，**只随产品发布编译成品，不公开源码**。
- **公开代码仓库**：正在调整、重建中；恢复后会在[开源说明页](https://leizai.cc/opensource.html)更新地址。
- **发布物完整性校验**：使用 Ed25519 验签，用于校验下载包与清单是否被篡改（私钥不在公开范围）。

---

## 链接

| | |
|---|---|
| 官网 | <https://leizai.cc> |
| 下载桌面版 | <https://leizai.cc/download.html> |
| 文档 | <https://leizai.cc/docs.html> |
| 定价 | <https://leizai.cc/pricing.html> |
| 开源说明 | <https://leizai.cc/opensource.html> |
| 问题反馈 | 本仓库 Issues |

---

## 联系与社群

有问题、想交流，欢迎扫码加入微信群：

![扫码加入微信群](docs/assets/wechat-group.jpg)

> 也可到本仓库 Issues 提问。
