# history-case-lab working rules

本仓库是“历史人生模拟 / history case lab”项目的正式工作仓库。以下规则适用于 AI 助手和人类协作者。

## 1. Source of truth

- **本仓库是唯一正式 source of truth。**
- `c3right/notepad` 中同名或相关笔记只视为历史快照，不得作为后续工作的依赖。
- 新结论、规则修订、案例状态、Packet 版本与路线更新，只在本仓库维护。
- 若发现旧笔记与本仓库冲突，以本仓库最新版本为准，并在 Revision log 说明重要变化。

## 2. 项目目标

核心问题：

> 如果我是历史当事人，在那个时刻，只拥有他当时能够拥有的信息，我会怎么选？

本项目不以成功学、英雄评判或事后解释为主要目标，而是建立可复用的“人生样本库”，训练有限信息、有限权限、时间压力、组织关系、风险、身份与价值冲突下的判断。

保持三轨：

- **D — Decision**：决策模拟；当前主建设轨。
- **L — Life-course**：人生历程模拟；不要强行寻找 Freeze。
- **W — World**：生活世界模拟；不要强行改造成选择题。

## 3. 目录职责

```text
README.md                 项目入口与当前状态
AGENTS.md                 本规则

docs/                     方法、路线、实验、跨案例研究记录
cases/<case-id>/           单案例正式工作区
  README.md                案例状态与入口
  research/                Atom、Qualification、Evidence Map 等研究视图
  packet/                  Reader Packet / Reveal / Prototype 版本
  sources/                 来源索引与材料地图；不存无授权全文
  tests/                   闭卷试读记录与反馈

templates/                 可复制模板
data/                      候选池、来源索引等结构化数据
archive/                   已废弃/冻结材料；不得作为活跃规则来源
```

已有从 `notepad` 迁入的阶段性文档保留在 `docs/`，以确保项目完全自包含。

## 4. 案例层级必须分开

始终区分：

> **Case Field → Case Episode → Decision Atom → Case Packet**

- 人物不是 Atom。
- 著名事件不是 Atom。
- 一本书不是 Atom。
- 一家公司或一场战争不是 Atom。
- **Decision Atom** 才是 D 轨最小准入、编码与评分单位。
- **Case Packet** 是人为制作的阅读产品，不是历史本体。

Sources 是另一棵树；一条来源可支持多个 Atom，一个 Atom 通常需要多个来源。

## 5. Decision Atom 基本定义

合格 Atom 应能写成：

> 在〔真实决策窗口〕，〔视角主体〕面对〔一个核心决策问题〕；基于其当时可获得的〔信息集〕，至少存在〔A/B……〕两个现实可行方案，而选择将影响〔主要利害〕。

优先遵循：

- `docs/2026-09-14-history-decision-atom-schema-v1.md`
- `docs/2026-09-14-history-decision-atom-scoring-v1.md`

除非多个异质样本重复暴露同一缺陷，不因单个精彩案例临时改规则。

## 6. Hard Gates 优先于软评分

Hard Gates 先判断“是不是可靠 Atom”；M01–M10 后判断“是否值得现在优先建设”。

不得：

- 用高戏剧性救回一个没有真实选项的案例；
- 用名气代替信息可重建度；
- 为了保留著名故事而降低 GATE；
- 因案例分数高就跳过主体、窗口、选项和证据审计。

Candidate 阶段只打 Provisional Score；Qualified 后才视为正式评分。

## 7. 主体边界必须和信息边界一致

不得把国家、公司、家庭自动拟人化。

至少区分需要时的：

- Focal Actor
- Formal Authority
- Effective Decider(s)
- Decision Group
- Veto / Constraint Holders
- Implementers
- Action Locus
- Deciders
- Affected Parties

不能让一个人物在 Packet 中拥有“组织全体知道的一切”。

## 8. Freeze 纪律

严格区分：

- Historical Event Node
- Decision Window
- Freeze Point
- Commitment Threshold

Freeze 应位于：

> **真实选择仍开放，但尚未越过主要承诺阈值的位置。**

著名签字日、开战日、辞职仪式、发布会往往已经太晚。

若无法恢复精确时刻，可明确使用 **Freeze Window / 操作性 Freeze**；不得伪造精确心理瞬间。

## 9. 选项纪律

选项按证据分级：

- **A**：明确被当事人考虑；
- **B**：强证据推定处于考虑范围；
- **C**：后人可想象的方案。

C 级不得与 A/B 等权进入 Freeze。

若 Reader Packet 列出选项，不得把作者偏好的方案写得明显更成熟、更细致，从而泄题。优先让读者自己形成方案。

## 10. Research View 与 Simulation View 分离

这是本仓库最重要的产品纪律之一。

### Research View

研究者可知道：

- 后来结果；
- 对手实际掌握的信息；
- 哪个情报后来证明错误；
- 长期后果与史学解释。

### Simulation View

Freeze 前只允许读者获得：

- 当时该视角主体能够合理获得的信息；
- 当时真实开放的选项与约束；
- 必要的背景。

**Research View 的知识不得偷渡到 Simulation View。**

## 11. B / P / N / R 来源角色

所有材料尽量标注用途：

- **B — Background**：制度、环境、人物关系与必要上下文；
- **P — Protagonist / Evidence**：恢复当事人信息、判断、选项、约束；
- **N — Narrative**：提供连续性与代入，不得小说化补心理；
- **R — Reveal / Review**：结果、后果、史学解释与复盘。

同一来源可以多角色，但需说明。

## 12. 证据纪律

- 同时代材料与后来回忆必须分开。
- 错误信息也是历史事实：若主体当时相信，应保留在 Simulation View。
- 不要因为某信息后来关键，就在 Freeze 前异常突出它。
- 不得用“他显然想到”“他一定意识到”等流畅叙事掩盖 Evidence Gap。
- later recollection 可以使用，但必须显式标注 Retrospective Evidence。
- 来源元数据若本身泄露未来，也应记录为 Packet 风险；**不得为了悬念伪造来源身份。**

## 13. 叙事污染审计

至少警惕：

- O — Outcome leakage
- C — Causal preloading
- M — Moral/personality labeling
- T — Teleology
- R — Retrospective reconstruction

Packet 还需警惕：

- **Analogical Contamination**：现代同构争论直接预装历史判断；
- **Source-Metadata Leakage**：材料年份或来源身份泄露未来。

处理原则：史料透明优先于悬念纯度。

## 14. Reveal 不是“正确答案”

Reveal 必须至少尽量分开：

1. 实际选择；
2. 执行与即时反馈；
3. 中长期后果；
4. 外部变量、运气与二阶效应；
5. 后世不同解释。

不得把“后来结果较好”直接反推为“当时决策必然正确”。

始终强调：

> **Outcome ≠ Decision Quality**

## 15. N 型案例额外规则

N（规范性困境）必须通过 Normative Open-Conflict Test：

> Freeze 时至少两项义务/价值仍被当事人本人认真承认，且优先关系尚未解决。

后世认为某人“应该”考虑的价值，不得自动算作当事人当时的真实义务。

## 16. 文件与版本规则

- 方法规范：`docs/*-schema-vN.md`、`docs/*-scoring-vN.md`。
- 实验/冲刺：保留版本号或序号，不覆盖关键历史实验。
- Case Packet：使用 `v0.x` 原型版本；完成实测和证据精校后再进入 `v1.0`。
- 重要文件保留 `Revision log` / `Version log`。
- 不静默改写一个已经用于实验的规则版本；重大修订创建新版本并说明差异。

## 17. Case workspace 规则

新案例一旦进入 Qualified 或准备深挖，应建立：

```text
cases/<case-id>/
├── README.md
├── research/
├── packet/
├── sources/
└── tests/
```

`README.md` 至少记录：

- 当前状态：candidate / qualified / packet-prototype / tested / archived；
- Focal Actor；
- Core Question；
- Freeze / Freeze Window；
- Primary Type；
- 主要证据缺口；
- 下一步。

## 18. 路线维护

项目阶段、当前优先级和下一小步统一维护在：

> `docs/2026-09-14-history-life-simulation-roadmap.md`

完成一项关键阶段后：

1. 更新路线图；
2. 更新相关案例 README；
3. 需要时更新 `data/candidates.yaml`；
4. 若产生新方法，不直接覆盖旧规则，先说明是否需要 v2。

## 19. 公开仓库安全

本仓库公开。不得存放：

- 密码、token、API key；
- 私密个人信息；
- 未授权的版权全文；
- 付费数据库导出的受限材料；
- 机密或专有资料。

对来源优先保存：书目信息、链接、页码、引用位置、简短摘录与研究笔记，而不是复制整本受版权保护作品。

## 20. 提交风格

直接提交到默认分支可接受，除非用户要求 PR。

推荐 commit message：

- `docs: add/update <method or roadmap>`
- `research: add <experiment or sprint>`
- `case: add/update <case-id> research`
- `packet: add/update <case-id> v0.x`
- `data: update candidate registry`
- `templates: add/update <template>`

## 21. 当前优先级

截至 2026-09-14：

1. **Starkloff 1918**：Packet Prototype v0.1 已完成；下一步首次闭卷试读。
2. **IBM / Learson 1962**：Qualified，Packet Feasibility = GREEN-；暂不抢在 Starkloff 试读前开工。
3. **Hirabayashi 1942**：Qualified，N-Gate = Medium，Packet Feasibility = AMBER-GREEN。
4. **Donner-Reed 1846**：重切后边缘 Qualified，后置。

当前原则：**先验证第一份产品，再扩大案例数量。**
