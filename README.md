# history-case-lab

一个面向“关闭上帝视角”的历史人生模拟研究项目。

核心问题不是“后来发生了什么”，而是：

> **如果我是当事人，在那个时刻，只拥有他当时能够拥有的信息，我会怎么选？**

本仓库是该项目的**正式工作仓库与唯一 source of truth**。项目相关规则、路线、实验、案例与 Case Packet 都在这里维护；不依赖 `c3right/notepad` 才能继续工作。

## 项目结构

```text
history-case-lab/
├── AGENTS.md                 # 仓库规则；AI 与人类协作者均应先读
├── README.md                 # 项目入口
├── docs/                     # 方法、路线、实验记录、已迁移历史文档
├── cases/                    # 各案例独立工作区
├── templates/                # Decision Atom / Qualification / Packet 等模板
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

## 关键文档

- [项目路线图与进展](./docs/2026-09-14-history-life-simulation-roadmap.md)
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

其他候选与排序见 `docs/2026-09-14-history-decision-atom-ranking-experiment-1.md`。

## 迁移说明

2026-09-14 以前该项目的阶段性产出最初保存在 `c3right/notepad`。这些项目相关文档已复制进入本仓库。自本仓库初始化起：

> **后续更新只维护 `history-case-lab`；`notepad` 中旧副本仅视为历史快照，不再作为依赖或权威版本。**

详细协作规则见 [AGENTS.md](./AGENTS.md)。
