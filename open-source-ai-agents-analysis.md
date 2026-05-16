# Open Source AI Agents & Dashboards Analysis

> 本文档分析 6 个开源 AI Agent 相关项目，涵盖 AI Agent 管理平台、群体智能引擎、Agent 指挥中心等多种类型。

---

## 项目总览

| 项目 | GitHub | Stars | 许可证 | 主要用途 |
|------|--------|-------|--------|----------|
| **Paperclip** | [paperclipai/paperclip](https://github.com/paperclipai/paperclip) | ⭐ 65.8k | MIT | 企业级 AI Agent 管理平台 |
| **MiroFish** | [666ghj/MiroFish](https://github.com/666ghj/MiroFish) | ⭐ 60.9k | - | 群体智能预测引擎 |
| **Multica** | [multica-ai/multica](https://github.com/multica-ai/multica) | ⭐ 28.8k | - | AI Agent 团队协作平台 |
| **OpenClaw Mission Control** | [abhi1693/openclaw-mission-control](https://github.com/abhi1693/openclaw-mission-control) | ⭐ 4k | MIT | 企业级 AI Agent 编排 Dashboard |
| **ClawPort** | [JohnRiceML/clawport-ui](https://github.com/JohnRiceML/clawport-ui) | ⭐ 875 | MIT | Claude Code Agent 团队命令中心 |
| **Mission Control** | [Capevace/mission-control](https://github.com/Capevace/mission-control) | ⭐ 12 | MIT | 实时 Dashboard 框架（已废弃）|

---

## 1. Paperclip

**GitHub**: https://github.com/paperclipai/paperclip  
**Stars**: 65,800 | **Forks**: 12,000 | **分支**: 327 | **提交**: 2,474

### 简介
Paperclip 是**开源的 AI Agent 工作管理平台**， tagline 为 "The open-source app everyone uses to manage agents at work"。它是本文档中 stars 最高的项目，表明其在社区中的高度认可。

### 技术栈

| 类别 | 技术 |
|------|------|
| 语言 | TypeScript |
| 运行时 | Node.js |
| 数据库 | PostgreSQL |
| 包管理 | pnpm (monorepo) |
| 部署 | Docker |
| 架构 | CLI + Server + UI |

### 核心功能

- **Agent 生命周期管理** - 完整的 Agent 创建、配置、监控能力
- **Skills 系统** - Agent 技能管理，支持自定义技能创建
- **CLI 工具** - 开发者友好的命令行界面
- **插件架构** - 扩展 Agent 能力
- **企业级架构** - PostgreSQL 后端、备份端点、安全修复

### 目录结构

```
paperclipai/paperclip/
├── cli/              # 命令行工具
├── server/          # 后端服务
├── ui/              # 用户界面
├── packages/        # 共享包
├── .agents/skills/  # Agent 技能定义
└── releases/        # 发布管理
```

### 适用场景

- 企业 AI Agent 部署与管理
- Agent 开发与测试
- 团队协作与工作流自动化
- 插件开发与功能扩展

### 优缺点

| ✅ 优势 | ⚠️ 劣势 |
|---------|---------|
| 最高 stars（65.8k），社区认可度高 | 全栈应用，设置复杂 |
| MIT 许可证，开源友好 | 需要 PostgreSQL 数据库 |
| 生产就绪架构（备份、安全修复） | 对简单用例可能过于复杂 |
| 活跃开发（2,474 次提交） | |

---

## 2. MiroFish

**GitHub**: https://github.com/666ghj/MiroFish  
**Stars**: 60,900 | **Forks**: 9,500 | **提交**: 260

### 简介
MiroFish 是一个**群体智能引擎**， tagline 为 "Rehearse the future in a digital sandbox, and win decisions after countless simulations"（在数字沙盒中排练未来，在无数次模拟中赢得决策）。

它从现实世界（突发新闻、政策草案、金融信号）提取种子信息，构建高保真平行数字世界，让数千个具有独立个性、长期记忆和行为逻辑的智能 Agent 交互进化。

### 技术栈

| 类别 | 技术 |
|------|------|
| 架构 | Backend + Frontend 分离 |
| 部署 | Docker & Docker Compose |
| 国际化 | 多语言支持（中英文） |
| API | LLM API 配置 |

### 核心功能

- **群体智能引擎** - 基于多 Agent 技术的预测系统
- **平行数字世界** - 高保真数字世界构建
- **Agent 模拟** - 数千个智能 Agent 具有独立个性
- **预测能力** - 未来轨迹预测、沙盒决策排练
- **数据注入** - "上帝视角"变量注入

### 适用场景

- 金融市场预测与趋势分析
- 政策影响模拟与分析
- 风险评估与建模
- 战略规划与情景推演
- 社会科学研究

### 优缺点

| ✅ 优势 | ⚠️ 劣势 |
|---------|---------|
| 独特概念：数字沙盒决策模拟 | 专业用例，较 niche |
| 高 stars（60.9k） | 提交次数较少（260），较新 |
| Docker 支持，易于部署 | 多 Agent 模拟需要专业知识 |
| 国际化的中英文文档 | |

---

## 3. Multica

**GitHub**: https://github.com/multica-ai/multica  
**Stars**: 28,800 | **Forks**: 3,500 | **分支**: 863 | **提交**: 3,063

### 简介
Multica 是一个**开源托管 Agent 平台**， tagline 为 "Turn coding agents into real teammates — assign tasks, track progress, compound skills"。

核心理念是将编码 Agent 变成真正的团队成员，可以分配任务、跟踪进度、累积技能。

### 技术栈

| 类别 | 技术 |
|------|------|
| 语言 | TypeScript/JavaScript |
| 前端 | Next.js (React) |
| 包管理 | pnpm (monorepo) |
| 部署 | Docker & Docker Compose |
| 架构 | 多包 monorepo |

### 核心功能

- **Agent 管理** - 创建和管理编码 Agent
- **Squads 系统** - 将 Agent 组织成"小队"协作
- **技能累积** - Agent 可以构建和共享技能
- **任务跟踪** - 实时任务进度监控
- **Token 使用追踪** - 按 issue 统计 token 消耗

### 目录结构

```
multica-ai/multica/
├── apps/           # 前端应用 (Next.js)
├── server/         # 后端服务
├── packages/       # 共享包
├── docker/         # Docker 配置
└── e2e/           # 端到端测试
```

### 适用场景

- 软件开发团队管理多个编码 Agent
- 构建 AI 优先的工程团队
- 任务自动化与 Agent 监督
- 多 Agent 工作流创建

### 优缺点

| ✅ 优势 | ⚠️ 劣势 |
|---------|---------|
| 活跃开发（3,000+ 提交） | Monorepo 结构复杂 |
| 完整的 Agent 生命周期管理 | 运行多 Agent 需较大计算资源 |
| 灵活部署（云或自托管） | |
| Docker 支持 | |
| 大社区（28.8k stars） | |

---

## 4. OpenClaw Mission Control

**GitHub**: https://github.com/abhi1693/openclaw-mission-control  
**Stars**: 4,000 | **提交**: 1,087 | **许可证**: MIT

### 简介
OpenClaw Mission Control 是一个**企业级 AI Agent 编排 Dashboard**，通过 OpenClaw Gateway 管理 AI Agent、分配任务、协调多 Agent 协作。

### 技术栈

| 类别 | 技术 |
|------|------|
| 架构 | Fullstack Monorepo |
| 后端 | Python |
| 前端 | 现代 Web 框架 |
| 部署 | Docker/Docker Compose |

### 核心功能

- **Work Orchestration** - 工作流程编排
- **Gateway 管理** - OpenClaw 网关管理
- **审批工作流** - 人工审批流程
- **多团队支持** - 企业级多团队管理

### 适用场景

- 企业 AI 运营
- 多团队 Agent 管理
- 需要治理和审批的工作流
- 大规模 Agent 部署

### 优缺点

| ✅ 优势 | ⚠️ 劣势 |
|---------|---------|
| MIT 许可证 | Stars 相对较低（4k） |
| 企业就绪（审批、多团队） | 主要面向 OpenClaw 生态 |
| 活跃开发（1,087 提交） | |

---

## 5. ClawPort

**GitHub**: https://github.com/JohnRiceML/clawport-ui  
**Stars**: 875 | **许可证**: MIT

### 简介
ClawPort 是** Claude Code Agent 团队的 AI Agent 命令中心**，基于 OpenClaw 构建。

### 技术栈

| 类别 | 技术 |
|------|------|
| 前端框架 | Next.js 16.1.6, React 19 |
| UI | Tailwind CSS 4, Radix UI |
| 图表 | @xyflow/react (React Flow) |
| 语言 | TypeScript |

### 核心功能

- **可视化组织图** - Agent 团队可视化
- **Agent 聊天** - 视觉/语音对话
- **看板面板** - 任务看板管理
- **定时任务监控** - Cron 作业监控
- **成本追踪** - Token/成本统计
- **实时活动控制台** - Agent 活动监控
- **记忆浏览器** - Agent 记忆查看

### 适用场景

- 使用 Claude Code + OpenClaw 的团队
- 需要可视化 Agent 监控的开发团队
- Agent 团队组织和任务管理

### 优缺点

| ✅ 优势 | ⚠️ 劣势 |
|---------|---------|
| 现代技术栈（Next.js 16, React 19） | Stars 较少（875） |
| 功能丰富的可视化界面 | 主要面向 Claude Code 用户 |
| MIT 许可证 | |

---

## 6. Mission Control (Capevace)

**GitHub**: https://github.com/Capevace/mission-control  
**Stars**: 12 | **许可证**: MIT | **状态**: ⚠️ 已废弃

### 简介
Capevace/mission-control 是一个**开源 JavaScript 实时 Dashboard 框架**，用于构建物联网和家庭自动化 Dashboard。

### 技术栈

| 类别 | 技术 |
|------|------|
| 后端 | Node.js, Express 5.0.0-beta.1 |
| 实时通信 | Socket.IO 4.0.0 |
| 认证 | Passport.js, bcrypt |
| 插件 | Spotify, HomeKit 等 |

### ⚠️ 警告

> **此项目已废弃** - 最后一次提交于 2022 年 2 月（4+ 年前）。不建议在新项目中使用。

### 适用场景

- **无** - 项目已废弃

### 优缺点

| ✅ 优势 | ⚠️ 劣势 |
|---------|---------|
| MIT 许可证 | ⚠️ 项目已废弃 |
| 插件架构 | 4+ 年无更新 |
| 实时通信 | 不建议使用 |

---

## 综合对比

### 功能对比

| 功能 | Paperclip | MiroFish | Multica | OpenClaw MC | ClawPort | Mission Control |
|------|-----------|----------|---------|-------------|----------|-----------------|
| **Agent 管理** | ✅ | ❌ | ✅ | ✅ | ✅ | ❌ |
| **多 Agent 协作** | ✅ | ✅ | ✅ | ✅ | ✅ | ❌ |
| **预测/模拟** | ❌ | ✅ | ❌ | ❌ | ❌ | ❌ |
| **可视化界面** | ✅ | ❌ | ✅ | ✅ | ✅ | ✅ |
| **企业级功能** | ✅ | ❌ | ❌ | ✅ | ❌ | ❌ |
| **CLI 工具** | ✅ | ❌ | ❌ | ❌ | ❌ | ❌ |
| **Docker 支持** | ✅ | ✅ | ✅ | ✅ | ❌ | ❌ |
| **MIT 许可证** | ✅ | ❌ | ❌ | ✅ | ✅ | ✅ |
| **活跃开发** | ✅ | ⚠️ | ✅ | ✅ | ⚠️ | ❌ |

### 选择指南

| 需求场景 | 推荐项目 |
|----------|----------|
| 企业级 Agent 管理 | **Paperclip** 或 **OpenClaw Mission Control** |
| AI 预测与模拟 | **MiroFish** |
| 编码 Agent 团队协作 | **Multica** |
| Claude Code Agent 可视化 | **ClawPort** |
| 通用 Dashboard 框架 | ~~Mission Control~~ (已废弃) |

---

## 总结

本次分析的 6 个开源项目覆盖了 AI Agent 领域的多个方向：

1. **Paperclip**（65.8k stars）- 最成熟、社区认可度最高的开源 Agent 管理平台，适合企业部署
2. **MiroFish**（60.9k stars）- 独特的群体智能预测引擎，适合需要模拟和预测的场景
3. **Multica**（28.8k stars）- 专注于将编码 Agent 变成团队成员，适合开发团队
4. **OpenClaw Mission Control**（4k stars）- 企业级 Agent 编排平台，适合大规模部署
5. **ClawPort**（875 stars）- 面向 Claude Code 的可视化命令中心
6. **Mission Control**（12 stars）- 已废弃，不建议使用

---

*文档生成时间: 2026-05-16*  
*分析工具: Hermes Agent*  
*目标仓库: Raostu/awesome-research*
