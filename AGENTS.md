# AGENTS.md - Agent 工作指南

本文档为 Agent（包括 CodeBuddy、Claude Code、Cursor、GitHub Copilot 等）在本仓库中工作提供指南。

## 核心记忆

### 项目定位

量潮学术研究（quanttide-research）是量潮知识管理体系中的**学术研究**领域第二大脑，涵盖学术成果、研究项目与学术交流等核心能力。

### 领域仓库统一结构

```
quanttide-research/
├── apps/              # 可部署应用（qt{产品名} / qtcloud-{产品名}）
├── packages/toolkit   # 共享库/工具集（独立仓库 quanttide-research-toolkit）
├── examples/default   # 实验室（独立仓库 quanttide-laboratory-of-academic-research）
├── data/              # 数据类资产（context/journal/intention/profile/roadmap/insight/brochure 等）
└── docs/              # 文档类资产（bylaw/handbook/specification/tutorial/essay/gallery）
```

## 人机协作范式

1. **最小干预**：仅在用户明确请求时操作
2. **信息复用**：优先使用已有文档内容
3. **维护记录**：修改后同步更新 CHANGELOG.md
4. **原子提交**：每次提交包含完整独立变更
5. **提交即推送**：提交后默认推送到远端，除非用户明确说"只提交不推"
