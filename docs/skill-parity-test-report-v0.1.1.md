# Skill 公开版差异测试报告 v0.1.1

测试日期：2026-04-28

## 测试范围

本轮用 4 个子代理分组测试公开版 Skill 和本地 Skill 的使用差异，重点看 4 件事：

- 公开版是否能独立使用。
- 是否暴露私有 reference、路径、案例或服务器信息。
- 是否缺少关键判断规则，导致输出明显弱于本地版。
- 是否适合作为第一批开源 Skill 发布。

## 分组结论

| 分组 | 测试对象 | 结论 | 本轮处理 |
|---|---|---|---|
| 私域 / 长文 | `insurance-private-domain-moments`、`wechat-article-chain-lite` | 可发布，但边界和 QA 不够 | 已补不适用场景、手机阅读、发布 QA、长文链路纪律和发布检查 |
| 内容诊断 / AI check | `cg-content-diagnosis-public`、`cg-ai-check-public` | `AI check` 需要补 reference 和误判规则 | 已补顾问口风 reference、10 条铁律、文体识别和误判提醒 |
| 商业 | `cg-business-diagnosis-lite`、`cg-problem-dissolver`、`business-insight-public` | 商业诊断 Lite 原本偏薄 | 已补产品存在性、价格判断、错误单位、商业轻检、路由边界和记录确认 |
| 会议 / 资料 / 调研 / 写作 | `meeting-notes`、`client-meeting-notes-public`、`kb-processor`、`deep-research-public`、`write-article-public` | 会议类较稳，调研和写作需补证据链 | 已补脱敏、客户状态理由、资料模式模板、调研类型、来源优先级、写作材料盘点和发布前检查 |

## AI Check reference 补充

新增公开安全文件：

- `skills/content-diagnosis/cg-ai-check-public/references/advisor-style-reference.md`

这份 reference 来自本地顾问内容口风规则的公开改写版，只保留通用表达原则：

- 客户视角优先。
- 不用恐吓式转化。
- 不把行业术语当专业感。
- 不暴露真实客户、内部项目、私有路径或成交数据。
- 输出时区分通用 AI 味问题和顾问场景口风问题。

## 和本地 Skill 的差别

公开版保留：

- 方法框架。
- 判断顺序。
- 输出结构。
- 常见误判提醒。
- 可替换占位符。

公开版不保留：

- 私有素材库。
- 真实客户案例。
- 内部 reference 原文。
- 自动化脚本路径。
- 服务器、API、Token、App ID、Secret。
- 只能在本人业务里使用的强风格规则。

## 当前可发布判断

第一批 `12` 个 Skill 可以继续作为公开版发布，但不应该全部当成拳头 Skill。

当前第一屏主推应聚焦 4 个拳头候选：

- `cg-ai-check-public`
- `cg-business-diagnosis-lite`
- `wechat-article-chain-lite`
- `insurance-private-domain-moments`

其余 Skill 作为配套工具或 Beta 工具存在。它们不是完整私有工作台的替代品，而是可自由下载、复制和改造的工作流骨架。

拳头标准见：

- `docs/flagship-standard.md`

## 后续观察

- `cg-content-diagnosis-public` 仍偏框架化，后续可补 3 个公开测试样例。
- `deep-research-public` 需要在真实调研任务中继续观察来源引用质量。
- `write-article-public` 可继续补 2-3 种文章结构模板，但不建议塞进主文件，后续放 `references/` 更合适。
