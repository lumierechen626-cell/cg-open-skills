# 拳头 Skill 标准

不是所有公开 Skill 都应该被包装成拳头。

公开仓库可以有工具型 Skill，但第一屏主推的拳头 Skill 必须满足更高标准。

## 拳头 Skill 必须具备

1. 有明确判断力，不只是流程模板。
2. 能处理误触发、边界场景和反例。
3. 主文件足够轻，但关键 reference 足够硬。
4. 有 3 个以上可复用测试样例。
5. 用户不用理解作者个人系统，也能独立使用。
6. 输出有明显差异感，不能像普通提示词合集。
7. 不能依赖私有素材库、真实案例、内部路径或个人记忆。

## 当前分层

### 拳头候选

这 4 个适合作为第一屏主推，但仍要继续补测试样例：

- `cg-ai-check-public`
- `cg-business-diagnosis-lite`
- `wechat-article-chain-lite`
- `insurance-private-domain-moments`

### 核心工具

这些可以放在第一批，但不抢主叙事：

- `cg-content-diagnosis-public`
- `cg-problem-dissolver`
- `meeting-notes`
- `client-meeting-notes-public`
- `kb-processor`
- `write-article-public`

### Beta 工具

这些可以发布，但要明确是轻量版，后续用真实任务继续打磨：

- `business-insight-public`
- `deep-research-public`

## 不够拳头的典型信号

- 只有步骤，没有判断。
- 输出结构很完整，但每一步都像常识。
- 没有说明什么时候不要用。
- 没有误判提醒。
- 没有测试样例。
- 看起来像“某个工作流的公开删减版”，而不是一个能独立产生价值的 Skill。

## 第一屏展示原则

README 第一屏只强调拳头候选，不把 12 个 Skill 平铺成同等重要。

完整清单可以保留，但要让用户一眼知道：

- 哪些是最值得下载体验的。
- 哪些是配套工具。
- 哪些还在 Beta。
