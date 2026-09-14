# history-case-lab

一个面向“关闭上帝视角”的历史人生模拟研究项目。

核心问题不是“后来发生了什么”，而是：

> **如果我是当事人，在那个时刻，只拥有他当时能够拥有的信息，我会怎么选？**

本仓库是该项目的**正式工作仓库与唯一 source of truth**。项目相关规则、路线、实验、案例与 Case Packet 都在这里维护；不依赖 `c3right/notepad` 才能继续工作。

## 项目结构

```text
history-case-lab/
├── AGENTS.md                 # 仓库规则；AI 与人类协作者均应先读
├── MIGRATION.md              # 从 notepad 独立出来的迁移记录
├── README.md                 # 项目入口
├── docs/                     # 方法、路线、实验记录、已迁移历史文档
├── cases/                    # 各案例独立工作区
├── templates/                # Decision Atom / Qualification / Packet / Test 模板
├── data/                     # 候选池、来源索引等结构化数据
└── archive/                  # 仅用于废弃/冻结材料；不得作为活跃规则来源
```

## 当前工作流

```text
D / L / W 定位
→ Case Field
→ Decision Atom
→ 主体 / 窗口 / 信息 / 选项审计
→ Hard Gates
→ M01–M10
→ Qualification Sprint
→ B/P/N/R 材料设计
→ Packet Feasibility
→ Case Packet Prototype
→ 闭卷试读
→ 复盘与迭代
```

当前 D 轨最成熟。L（Life-course）和 W（World）保留为后续建设方向。

## 从哪里开始

- **项目规则**：[AGENTS.md](./AGENTS.md)
- **迁移与 source-of-truth 说明**：[MIGRATION.md](./MIGRATION.md)
- **文档目录**：[docs/INDEX.md](./docs/INDEX.md)
- **项目路线图与当前下一步**：[docs/2026-09-14-history-life-simulation-roadmap.md](./docs/2026-09-14-history-life-simulation-roadmap.md)
- **案例工作区**：[cases/](./cases/)
- **可复用模板**：[templates/](./templates/)
- **候选案例注册表**：[data/candidates.yaml](./data/candidates.yaml)

## 关键方法文档

- [Decision Atom 正式字段表 v1](./docs/2026-09-14-history-decision-atom-schema-v1.md)
- [Decision Atom 软评分量表 v1](./docs/2026-09-14-history-decision-atom-scoring-v1.md)
- [第一次候选排序实验](./docs/2026-09-14-history-decision-atom-ranking-experiment-1.md)
- [Qualification Sprint 1](./docs/2026-09-14-history-decision-atom-qualification-sprint-1.md)
- [首批 Case Packet Feasibility Mini-Design](./docs/2026-09-14-history-case-packet-feasibility-mini-design-1.md)
- [Starkloff Case Packet Prototype v0.1](./docs/2026-09-14-history-case-packet-starkloff-v0.1.md)

## 当前案例状态

- **Starkloff / St. Louis 1918** — Qualified；Packet Prototype v0.1 已完成，下一步闭卷试读。
- **IBM / Vin Learson 1962** — Qualified；Packet Feasibility = GREEN-。
- **Gordon Hirabayashi 1942** — Qualified；N-Gate = Medium；Packet Feasibility = AMBER-GREEN。
- **Donner-Reed 1846** — 原切法否决；重切后边缘 Qualified，后置。

其他候选与排序见 [candidate registry](./data/candidates.yaml) 与第一次排序实验。

## 迁移说明

2026-09-14 以前该项目的阶段性产出最初保存在 `c3right/notepad`。项目相关的七份核心产出已经完整复制进入本仓库；另外建立了本地案例工作区、模板、候选注册表与迁移记录。

原 Decision Atom 文档曾引用两个宏观历史阅读框架。它们不是运行本项目所必需的依赖；本仓库已保留本地 context stub，确保项目规则、路线、案例与 Packet 均可在本仓库独立理解和继续开发。

自本仓库初始化起：

> **后续更新只维护 `history-case-lab`；`notepad` 中旧副本仅视为历史快照，不再作为依赖或权威版本。**
