# AI Venture Studio Governance

**File:** `docs/06-governance/GOVERNANCE.md`  
**Version:** v0.1  
**Status:** Draft  
**Owner:** muxing dai

---

## 1. Purpose

Governance 是 AI Venture Studio 的治理体系，负责保证 AI Venture Studio 的所有决策符合 Mission、Constitution 和长期发展方向。
AI BOS 负责执行 Governance。

Governance 不负责执行任务。

Governance 的职责是：

- 判断是否应该做；
- 判断是否应该继续；
- 判断是否应该停止；
- 判断是否应该修改系统。

---

## 2. Governance Layers

AI BOS 采用四层治理模型：

```text
Mission Governance
        ↓
Architecture Governance
        ↓
Business Governance
        ↓
Execution Governance
```

任何重大决策都必须依次经过对应层级。

---

## 3. Mission Governance

### 职责

确认所有 Opportunity、Experiment、Framework、系统修改是否符合 Mission。

### 核心问题

- 是否符合 AI Venture Studio Mission？
- 是否符合长期价值？
- 是否符合可持续发展方向？
- 是否有助于资产沉淀？

如果答案是否，则停止进入下一层。

---

## 4. Architecture Governance

### 职责

保护 AI BOS 的长期结构稳定。

Architecture Governance 不讨论商业价值，只讨论系统结构。

### 核心问题

- 是否破坏现有架构？
- 是否违反 Constitution？
- 是否应该新增 Framework？
- 是否应该修改已有 Specification？
- 是否需要 ADR？

任何 Architecture 修改，都必须留下 ADR。

---

## 5. Business Governance

### 职责

管理商业机会生命周期。

负责：

- 是否值得验证；
- 是否继续投入；
- 是否暂停；
- 是否 Kill；
- 是否进入 Scale。

Business Governance 的判断依据来自：

- Opportunity Engine
- 实验数据
- 客户反馈
- 商业指标

---

## 6. Execution Governance

### 职责

负责执行层资源协调。

包括：

- Role 分配；
- Agent 选择；
- 工作顺序；
- 自动化触发；
- Workspace 生命周期管理。

Execution Governance 不得修改 Mission、Constitution 或 Architecture。

---

## 7. Governance Decision Levels

所有决策划分为三个等级。

### Level 1：Operational

日常执行决策。

例如：

- 今天先联系哪位客户；
- 哪个 AI 执行任务；
- 今天完成哪些实验。

无需修改系统。

---

### Level 2：Business

商业方向决策。

例如：

- 是否继续某个 Experiment；
- 是否建立新的 Framework；
- 是否停止一个方向。

可能产生新的资产。

---

### Level 3：System

系统级决策。

例如：

- 修改 Constitution；
- 修改 Architecture；
- 修改 Governance；
- 新增核心对象。

必须经过：

```text
Proposal → Review → ADR → Release
```

---

## 8. Governance Principles

AI Venture Studio Governance 永远遵守：

1. Mission 优先；
2. 长期价值优先；
3. 事实优先；
4. Opportunity 优先；
5. 资产优先；
6. Governance 高于 Agent；
7. Rule 高于 Model。

---

## 9. Governance Outputs

Governance 每次只能输出以下结果之一：

- APPROVE：批准；
- HOLD：暂缓；
- REJECT：拒绝；
- KILL：终止；
- SCALE：进入规模化。

不得输出模糊结论。

---

## 10. Relationship with AI Agents

任何 AI Agent 都不能拥有 Governance。

AI Agent 只能：

- 提供分析；
- 提供建议；
- 提供预测。

最终治理依据始终来自 Governance Rules，而不是模型本身。

---

## 11. Relationship with ADR

任何 Governance 引发的系统修改，都必须形成 ADR。

ADR 是 AI BOS 的唯一正式决策记录。

---

## 12. Current Status

当前版本：v0.1 Draft

属于 Epic-001：Foundation。

待与 Architecture-001 完成一致性检查后升级为 v1.0。
