# AI BOS

AI BOS（AI Business Operating System）是一套用于持续发现、验证、复制和放大商业机会的 AI 公司操作系统。

它不是一个单一项目，也不是某个 Prompt 集合，而是一套可长期演进的商业操作系统，用来管理机会、实验、知识资产、决策记录、工作流和 AI Agent 协作。

---

## 1. Mission

打造一套能够持续发现、验证、复制和放大商业机会的 AI 商业体系，让个人和未来团队都能以最低成本、最快速度，把一个想法变成真实价值，并不断沉淀可复用的能力资产。

---

## 2. Core Philosophy

AI BOS 的核心思想：

1. 资产比项目重要。
2. 岗位比模型重要。
3. 机会比任务重要。
4. 验证比想象重要。
5. 推进比回答重要。
6. 规则比模型重要。
7. 系统必须独立于任何单一 AI、平台或聊天窗口。

---

## 3. What AI BOS Is

AI BOS 是一个用于管理 AI Company 的操作系统。

它负责：

* 发现商业机会；
* 评估机会是否值得验证；
* 管理商业实验；
* 调度不同 AI Agent；
* 管理 Workspace 状态；
* 沉淀 Framework、SOP、Template、Case、Automation 等长期资产；
* 记录重要架构决策；
* 让个人和未来团队在同一套规则下工作。

---

## 4. What AI BOS Is Not

AI BOS 不是：

* 一个普通项目文件夹；
* 一个 Prompt 仓库；
* 一个单一 AI 工具；
* 一个聊天记录合集；
* 一个任务清单系统；
* 一个只服务某个项目的 SOP。

AI BOS 是一套长期可复用、可升级、可扩展的 AI 商业操作系统。

---

## 5. System Hierarchy

```text
Life Mission
    ↓
AI Company
    ↓
AI BOS
    ↓
Opportunity Portfolio
    ↓
Opportunity Engine
    ↓
Business Framework
    ↓
Workspace / Experiment
    ↓
Execution
    ↓
Assets
```

---

## 6. Core Objects

### 6.1 Opportunity

Opportunity 是 AI BOS 的核心工作单元。

它不是一个普通想法，而是一个值得验证的商业假设。

每一个 Opportunity 都必须拥有：

* ID
* Title
* Source
* Pain
* Value
* Mission Fit
* Status

未经 Opportunity Engine 审核的想法，不允许进入执行。

---

### 6.2 Workspace

Workspace 是一个商业实验的运行环境。

每个 Workspace 必须有唯一的 `STATE.md`，作为该实验的唯一事实源。

Workspace 不等于项目。

Workspace 的目标不是“完成项目”，而是验证商业假设，并沉淀可复用资产。

---

### 6.3 Asset

Asset 是 AI BOS 的长期复利来源。

Asset 包括：

* Framework
* SOP
* Template
* Case Study
* Automation
* Dataset
* Specification
* ADR
* Knowledge Entry

任何实验结束后，都必须回答：

> 这个实验为 AI BOS 新增了什么资产？

---

### 6.4 Role

AI BOS 只绑定 Role，不绑定具体模型。

例如：

```text
Strategist → 当前可由 GPT 担任
Writer → 当前可由 Claude 担任
Executor → 当前可由 DeepSeek 担任
Engineer → 当前可由 Codex 担任
Project Manager → 当前可由 Hermes 担任
```

模型可以替换，Role 保持稳定。

---

## 7. Constitution Draft

当前已确认的宪法原则：

### Constitution #1：先立项，后执行

任何项目进入执行之前，必须先完成 Opportunity Engine 的立项审批。

未经审批，不得创建 Workspace，不得分配任务，不得进入开发或执行。

---

### Constitution #2：事实优先，推理其次

任何 AI 在提供建议、制定计划或执行任务之前，必须先读取当前 Workspace 的 `STATE.md`。

`STATE.md` 是唯一事实源。

---

### Constitution #3：推进优先，不回答优先

AI 的第一职责不是回答问题，而是推动当前 Workspace 向下一阶段前进。

任何回复都必须服务于项目推进，而不是制造信息过载。

---

### Constitution #4：岗位优先，模型其次

AI BOS 永远绑定 Role，不绑定具体 AI 模型。

模型可以替换，岗位职责保持稳定。

---

### Constitution #5：治理优先

任何机会、决策、实验、Framework 修改，都必须先经过 Governance，而不是直接进入执行。

---

## 8. Governance

AI BOS 的治理分为四层：

```text
Mission Governance
    ↓
Architecture Governance
    ↓
Business Governance
    ↓
Execution Governance
```

### Mission Governance

判断某个机会、决策或实验是否符合 Mission。

不符合 Mission 的机会，不进入系统。

### Architecture Governance

判断某个修改是否会破坏 AI BOS 的长期结构。

### Business Governance

判断某个机会是否值得验证、继续、暂停或放大。

### Execution Governance

决定具体由哪个 Role / Agent 执行任务。

---

## 9. Opportunity Pipeline

Opportunity 的生命周期：

```text
Captured
    ↓
Qualified
    ↓
Experiment
    ↓
Validated
    ↓
Assetized
    ↓
Scaled
```

每个阶段之间都必须经过 Gate。

---

## 10. Gate 1：Idea → Opportunity

Gate 1 的职责不是判断项目是否值得做，而是判断一个模糊想法能不能成为一个真正的 Opportunity。

必须检查：

1. Source：是否有真实来源；
2. Pain：是否存在真实痛点；
3. Value：是否存在明确价值交换；
4. Mission Fit：是否符合 Mission；
5. Validation Worthiness：是否值得做一次低成本验证。

Gate 1 输出只有三种：

```text
PASS
HOLD
REJECT
```

---

## 11. AI BOS Design System

AI BOS 不能随意修改。

所有重要变更必须经过：

```text
Proposal
    ↓
Review
    ↓
ADR
    ↓
Release
```

系统永远不直接修改，只能通过版本演进。

---

## 12. ADR

ADR 是 Architecture Decision Record。

用于记录重要架构决策。

每个 ADR 必须说明：

* 决策是什么；
* 为什么做这个决策；
* 为什么不采用其他方案；
* 会影响哪些模块；
* 当前状态。

示例：

```text
ADR-001
Title: Opportunity Portfolio 成为 AI Company 一级对象
Status: Accepted
```

---

## 13. Repository Structure

当前建议目录结构：

```text
ai-bos/
│
├── README.md
│
├── mission/
│   └── MISSION.md
│
├── constitution/
│   └── CONSTITUTION.md
│
├── architecture/
│   └── ARCH-001-ai-company-context.md
│
├── governance/
│   └── GOVERNANCE.md
│
├── adr/
│   └── ADR-001-opportunity-portfolio.md
│
├── specifications/
│   └── SPEC-OE-001-opportunity-gate-1.md
│
├── frameworks/
│
├── roles/
│
├── workspaces/
│
├── knowledge/
│
├── templates/
│
├── assets/
│
└── archive/
```

---

## 14. Current Status

当前 AI BOS 处于早期架构设计阶段。

已完成：

* Mission 初步确认；
* AI Company 概念确认；
* AI BOS 与 AI Company 分层确认；
* Opportunity 作为核心对象确认；
* Opportunity Portfolio 概念确认；
* Gate 1 初步规范确认；
* Governance 四层结构确认；
* ABDS（AI BOS Design System）初步确认；
* Git 管理方案确认。

---

## 15. Next Step

下一步：

创建正式目录结构，并沉淀第一批核心文档：

1. `MISSION.md`
2. `CONSTITUTION.md`
3. `ARCH-001-ai-company-context.md`
4. `GOVERNANCE.md`
5. `ADR-001-opportunity-portfolio.md`
6. `SPEC-OE-001-opportunity-gate-1.md`

---

## 16. Operating Rule

以后任何新想法、项目、实验，都必须先回答：

```text
这是不是一个 Opportunity？
它是否通过 Gate 1？
它属于哪个 Business Framework？
它是否值得创建 Workspace？
它能沉淀什么 Asset？
```

如果回答不清楚，不允许进入执行。

---

## 17. Owner

Owner：muxing dai

AI BOS 当前阶段由 Owner 与 AI 商业导师共同设计，未来支持团队、多个 AI Agent、多项目并行运行。
