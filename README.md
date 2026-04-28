# CG Open Skills

一组可自由下载、复制和改造的 Agent Skill。

这不是一个课程，也不是一个终端产品。这里放的是一批已经在真实内容生产、商业诊断、会议纪要和资料整理中反复使用过的工作流骨架。公开版只保留通用方法、判断流程和输出结构，不包含私有素材库、真实客户案例、API、服务器配置或内部 SOP。

## 第一批 Skill

| 分类 | Skill | 适合场景 |
|---|---|---|
| 私域内容 | `insurance-private-domain-moments` | 保险人 / 顾问的朋友圈内容，覆盖 B 端交付、C 端咨询和价值圈 |
| 长文链路 | `wechat-article-chain-lite` | 公众号长文从选题到发布态的轻量工作链 |
| 内容诊断 | `cg-content-diagnosis-public` | 判断一个选题或文案该不该做、怎么做、哪里会写空 |
| AI 检查 | `cg-ai-check-public` | 检查文案里的 AI 味、解释腔、套路感和过度光滑 |
| 商业诊断 | `cg-business-diagnosis-lite` | 用问诊方式拆商业问题，而不是直接给答案 |
| 问题消解 | `cg-problem-dissolver` | 把模糊问题改写成可验证问题 |
| 商业灵感 | `business-insight-public` | 把零散商业想法沉淀成可讨论记录 |
| 会议纪要 | `meeting-notes` | 把会议文本、录音转写、零散笔记整理成纪要 |
| 客户面谈 | `client-meeting-notes-public` | 把客户沟通记录整理成需求、顾虑和下一步动作 |
| 知识处理 | `kb-processor` | 把 PDF、截图、录音、文档整理成结构化知识 |
| 深度调研 | `deep-research-public` | 多源调研、证据池、事实核验和输出报告 |
| 长文写作 | `write-article-public` | 深度文章、观点文、公众号长文的写作工作流 |

## 怎么用

1. 下载整个仓库，或只下载你需要的单个 Skill。
2. 找到对应目录下的 `SKILL.md`。
3. 复制到你使用的 Agent / Codex / Claude / Hermes 的 skills 目录。
4. 根据你的业务，把 `{你的品牌}`、`{你的行业}`、`{你的用户}` 等占位符替换掉。

详细说明见 [docs/install.md](docs/install.md)。

## 开源边界

公开版已经做过脱敏处理：

- 不包含真实客户、真实学员或真实成交案例。
- 不包含本地绝对路径。
- 不包含 API Key、Token、Secret、App ID、服务器地址。
- 不包含私有素材库和内部 reference。
- 不承诺生成内容一定带来转化。

更多边界见 [docs/safety.md](docs/safety.md)。

## 国内下载

GitHub 是主仓库。国内镜像、飞书下载页和 zip 包说明见 [docs/download.md](docs/download.md) 与 [docs/domestic-mirror.md](docs/domestic-mirror.md)。

## 许可证

默认采用 MIT License。你可以复制、修改、分发和商用，但请自行承担使用结果，并不要把示例当成专业法律、财税、医疗或投资建议。
