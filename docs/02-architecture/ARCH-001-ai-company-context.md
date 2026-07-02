# ARCH-001 — AI Venture Studio Context

**File:** `docs/02-architecture/ARCH-001-ai-company-context.md`  
**Version:** v0.1  
**Status:** Draft  
**Owner:** muxing dai

---

## 1. Purpose

本架构定义 AI Venture Studio 的最高层结构，以及各核心对象之间的关系。

本文件不描述内部实现，只描述系统边界与职责。

---

## 2. Core Principle

AI Venture Studio 是商业组织。

AI BOS 是 AI Venture Studio 的操作系统。

AI Agent 是执行者。

Workspace 是实验运行环境。

Asset 是长期沉淀结果。

---

## 3. Context Architecture

```text
                    CEO（Owner）
                          │
                          ▼
                    AI Venture Studio
                          │
      ┌───────────────────┼───────────────────┐
      │                   │                   │
      ▼                   ▼                   ▼
 Mission             Governance         Opportunity Portfolio
      │                                       │
      └──────────────────────┬────────────────┘
                             ▼
                    Opportunity Engine
                             │
                      PASS / HOLD / REJECT
                             │
                             ▼
                         AI BOS
                             │
          ┌──────────────────┼──────────────────┐
          │                  │                  │
          ▼                  ▼                  ▼
     Business           Workspace           Knowledge
     Frameworks       (Experiments)          Assets
          │                  │                  │
          └──────────────────┼──────────────────┘
                             ▼
                      AI Agent Roles
                             │
                             ▼
                        External World
```

---

## 4. Layer Responsibilities

### Layer 1 — CEO

负责：

- 制定 Mission；
- 最终承担责任；
- 批准重大商业方向。

CEO 不负责具体执行。

---

### Layer 2 — AI Venture Studio

负责：

- Mission
- Constitution
- Governance
- Organization

AI Venture Studio 是最高商业实体。

---

### Layer 3 — Opportunity Portfolio

负责管理所有待评估商业机会。

这里保存：

- 新发现机会；
- 待验证机会；
- 已暂停机会。

Opportunity Portfolio 不负责执行。

---

### Layer 4 — Opportunity Engine

Opportunity Engine 是 AI Venture Studio 的唯一正式入口。

职责：

- 判断是否构成 Opportunity；
- 执行各 Gate；
- 决定是否进入 AI BOS。

未经 Opportunity Engine，不允许进入执行。

---

### Layer 5 — AI BOS

AI BOS 是执行操作系统。

负责：

- 调度 Framework；
- 创建 Workspace；
- 调度 Role；
- 管理 Assets；
- 推进 Experiment。

---

### Layer 6 — Business Framework

每个 Opportunity 必须匹配一个 Business Framework。

Framework 定义：

- 验证方式；
- 商业规则；
- Gate；
- SOP；
- 指标。

Framework 是长期资产。

---

### Layer 7 — Workspace

Workspace 是一个 Experiment 的运行环境。

每个 Workspace 必须拥有唯一 STATE。

STATE 是唯一事实源。

---

### Layer 8 — Knowledge Assets

长期资产包括：

- Framework
- SOP
- Template
- ADR
- Specification
- Case Study
- Automation
- Dataset
- Knowledge

任何 Experiment 都应新增或优化至少一种资产。

---

### Layer 9 — AI Agent Roles

AI BOS 永远绑定 Role，不绑定模型。

例如：

- Strategist
- Researcher
- Project Manager
- Engineer
- Writer
- Growth
- Knowledge Manager

具体由 GPT、Claude、Hermes、Codex、DeepSeek 等担任，是运行时配置。

---

## 5. Architecture Rules

1. AI Venture Studio 高于 AI BOS。
2. AI BOS 高于任何 Agent。
3. Opportunity 必须先进入 Portfolio。
4. Opportunity Engine 是唯一正式入口。
5. Workspace 只能由 AI BOS 创建。
6. Asset 永远属于 AI Venture Studio，不属于单一 Workspace。
7. Agent 可替换，Role 不可替换。

---

## 6. Out of Scope

以下内容不属于本架构：

- Opportunity 数据结构；
- Gate 详细规则；
- Framework 内部设计；
- Role 详细职责；
- Orchestrator；
- Dashboard。

这些将在后续 Architecture 中定义。

---

## 7. Related Documents

- `docs/01-foundation/mission/MISSION.md`
- `docs/01-foundation/PRODUCT-DEFINITION.md`
- `docs/01-foundation/constitution/CONSTITUTION.md`
- `docs/06-governance/GOVERNANCE.md`

---

## 8. Current Status

Architecture Version：v0.1 Draft

Epic：Foundation

Review Status：Pending
