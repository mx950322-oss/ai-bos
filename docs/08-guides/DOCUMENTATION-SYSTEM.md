# AI BOS Documentation System

**File:** `docs/08-guides/DOCUMENTATION-SYSTEM.md`  
**Version:** v0.1  
**Status:** Draft  
**Owner:** muxing dai

---

## 1. Purpose

Documentation System 定义 AI BOS 所有正式文档的管理规则。

它回答四个问题：

1. 什么文档可以进入 Git？
2. 文档如何组织？
3. 文档如何演进？
4. 哪份文档拥有最高权威？

Documentation System 的目标不是保存 Markdown，而是建立 AI Venture Studio 的知识资产体系。

---

## 2. Documentation Hierarchy

所有正式文档分为八类：

```text
01 Foundation
02 Architecture
03 Specification
04 Framework
05 Workspace Guide
06 Governance
07 Decision
08 Guide
```

每类文档职责固定，不允许混用。

---

## 3. 01 Foundation

Foundation 定义 AI Venture Studio 永久不变的核心原则。

包括：

- Mission
- Product Definition
- Constitution
- Vision（未来）
- Core Values（未来）

特点：

- 更新频率最低；
- 修改成本最高；
- 必须经过 ADR。

---

## 4. 02 Architecture

Architecture 描述系统结构。

例如：

- Context Diagram
- Operating Model
- Opportunity Engine
- Orchestrator

Architecture 不描述具体实现。

---

## 5. 03 Specification

Specification 描述具体规则。

例如：

- Opportunity Gate
- Data Model
- API
- Workflow
- Validation Rules

Specification 必须能够直接指导实现。

---

## 6. 04 Framework

Framework 是可复用的商业方法。

例如：

- Outbound Framework
- SaaS Validation Framework
- Local Business Growth Framework

Framework 来源于真实商业验证。

未经验证的方法不得称为 Framework。

---

## 7. 05 Workspace Guide

Workspace Guide 定义 Workspace 的规范。

注意：

Workspace 的运行状态（STATE）属于 Runtime，不进入 Git。

Git 中只保存 Workspace 的标准、模板和说明。

---

## 8. 06 Governance

Governance 定义治理规则。

包括：

- Governance Structure
- Decision Levels
- Approval Rules
- Change Process

Governance 负责保护 AI BOS 的长期稳定。

---

## 9. 07 Decision

Decision 使用 ADR（Architecture Decision Record）。

每一个重大决策都必须记录：

- Decision
- Context
- Alternatives
- Reason
- Impact
- Status

ADR 是唯一正式决策记录。

---

## 10. 08 Guide

Guide 提供使用说明。

例如：

- Session Start Guide
- Git Workflow
- AI Agent Onboarding
- Team Onboarding

Guide 可以修改，但必须保持与 Foundation 一致。

---

## 11. Document Lifecycle

所有正式文档统一采用以下生命周期：

```text
Draft
    ↓
Review
    ↓
Approved
    ↓
Released
    ↓
Deprecated（可选）
    ↓
Archived
```

说明：

- Draft：正在编写；
- Review：等待评审；
- Approved：评审通过；
- Released：正式生效；
- Deprecated：停止维护，但仍可参考；
- Archived：归档，不再使用。

---

## 12. Document Header Standard

所有正式文档统一包含以下信息：

```text
Title
File
Version
Status
Owner
Last Updated（可选）
Related Documents
```

任何正式文档不得省略 Version 和 Status。

---

## 13. Source of Truth

AI BOS 采用唯一事实源原则。

### Git Repository

负责保存：

- Mission
- Product Definition
- Constitution
- Architecture
- Governance
- Framework
- Specification
- ADR
- Guide

这些属于长期资产。

### Runtime

负责保存：

- Workspace State
- Experiment Progress
- Daily Tasks
- Temporary Notes

Runtime 不属于 Git。

---

## 14. Versioning Rules

Version 使用：

```text
v0.x
探索阶段

v1.x
正式发布

v2.x
重大升级
```

重大结构调整必须新增版本，而不是覆盖旧版本。

---

## 15. Documentation Principles

Documentation 永远遵守：

1. 文档服务系统，不服务聊天；
2. Git 保存长期资产；
3. Runtime 保存运行状态；
4. 文档优先于记忆；
5. Architecture 优先于 Specification；
6. Foundation 优先于一切。

---

## 16. Epic Completion Rule

一个 Epic 只有满足以下条件才允许 Release：

- 所有计划文档完成；
- Architecture Review 通过；
- ADR 已更新（如需要）；
- 文档状态更新为 Approved；
- Git 提交完成；
- 发布版本号。

---

## 17. Current Status

Version：v0.1 Draft

Epic：Foundation

Review Status：Pending
