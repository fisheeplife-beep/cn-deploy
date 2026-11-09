# cn-deploy

中文可跟做部署指南合集（配套开源仓索引）。

上游热门工具缺完整中文部署资料时，这里提供：**实测步骤 + 脚本 + 国内网络说明**。先跑 [cn-deploy-doctor](https://github.com/fisheeplife-beep/cn-deploy-doctor) 体检，再用 [trending-gap-radar](https://github.com/fisheeplife-beep/trending-gap-radar) 找选题。

## 工具

| 仓库 | 用途 |
|------|------|
| [cn-deploy-doctor](https://github.com/fisheeplife-beep/cn-deploy-doctor) | 国内环境部署体检 |
| [trending-gap-radar](https://github.com/fisheeplife-beep/trending-gap-radar) | 中文部署缺口选题雷达 |

## 部署配套

| 上游 | 配套仓 | 状态 |
|------|--------|------|
| [paperclipai/paperclip](https://github.com/paperclipai/paperclip) | [cn-deploy-paperclip](https://github.com/fisheeplife-beep/cn-deploy-paperclip) | CLI 已实测 |
| [vercel-labs/agent-browser](https://github.com/vercel-labs/agent-browser) | [cn-deploy-agent-browser](https://github.com/fisheeplife-beep/cn-deploy-agent-browser) | CLI + Chrome doctor 已实测 |
| [milind-soni/OpenMausBot](https://github.com/milind-soni/OpenMausBot) | [cn-deploy-openmausbot](https://github.com/fisheeplife-beep/cn-deploy-openmausbot) | CLI serve 已实测 |
| [lightpanda-io/browser](https://github.com/lightpanda-io/browser) | [cn-deploy-lightpanda](https://github.com/fisheeplife-beep/cn-deploy-lightpanda) | 二进制 1.0.0 + CDP + Puppeteer 已实测 |
| [JetBrains/thinkrail](https://github.com/JetBrains/thinkrail) | [cn-deploy-thinkrail](https://github.com/fisheeplife-beep/cn-deploy-thinkrail) | CLI stable 0.3.0 安装+host UI 已实测 |
| [melgarafael/DeskcommCRM](https://github.com/melgarafael/DeskcommCRM) | [cn-deploy-deskcommcrm](https://github.com/fisheeplife-beep/cn-deploy-deskcommcrm) | GHCR 探针已验证；VPS install 待有 Docker 的机器实测 |
| [firecrawl/firecrawl](https://github.com/firecrawl/firecrawl) | [cn-deploy-firecrawl](https://github.com/fisheeplife-beep/cn-deploy-firecrawl) | GHCR pull + Compose 起栈 + readiness 已实测；**/v2/scrape 沙箱桥接未跑通** |
| [openclaw/openclaw](https://github.com/openclaw/openclaw) | [cn-deploy-openclaw](https://github.com/fisheeplife-beep/cn-deploy-openclaw) | GHCR pull + 非交互 onboard + Compose 起 Gateway + healthz/Control UI 已实测；**真实模型对话/IM 未验证** |
| [n8n-io/n8n](https://github.com/n8n-io/n8n) | [cn-deploy-n8n](https://github.com/fisheeplife-beep/cn-deploy-n8n) | 钉版本 2.46.4 pull + **SQLite Compose `/healthz`/编辑器已实测**；Postgres+runners 起栈，**桥接 TCP 未跑通**；反代/Webhook/升级清单已文档化 |
| [dsx-ai-factory/nvke](https://github.com/dsx-ai-factory/nvke) | [cn-deploy-nvke](https://github.com/fisheeplife-beep/cn-deploy-nvke) | 钉 v0.23.1：浅克隆 + CAPNICo download + **nvkectl 已实测**；kind/Tilt/mock-NICo 全栈与裸金属 NICo **未验证**（作者机无 Docker，内存头寸不足 12GiB 空闲） |

## AI短剧

音频驱动口型 / 长对白说话镜头 / 多人对话 / 成片后期修口型等短剧相关配套：

| 上游 | 配套仓 | 状态 |
|------|--------|------|
| [MeiGen-AI/MultiTalk](https://github.com/MeiGen-AI/MultiTalk) | [cn-deploy-multitalk](https://github.com/fisheeplife-beep/cn-deploy-multitalk) | 预检+浅克隆 layout 已实测；**GPU 推理 Not verified**（作者机无 NVIDIA） |
| [MeiGen-AI/InfiniteTalk](https://github.com/MeiGen-AI/InfiniteTalk) | [cn-deploy-infinitetalk](https://github.com/fisheeplife-beep/cn-deploy-infinitetalk) | 预检+浅克隆 layout 已实测；**GPU 推理 Not verified**（作者机无 NVIDIA） |
| [bytedance/LatentSync](https://github.com/bytedance/LatentSync) | [cn-deploy-latentsync](https://github.com/fisheeplife-beep/cn-deploy-latentsync) | 预检+浅克隆 layout 已实测；**GPU 推理 Not verified**（作者机无 NVIDIA） |

## 原则

1. 先实测再写步骤  
2. 标明上游，不整页搬运 README  
3. 国内镜像 / 代理 / 弱网单独成章  
4. 未验证项明确写出  

## License

各子仓以各自 LICENSE 为准；本索引 MIT。
