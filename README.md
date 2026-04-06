# Awesome Research - AI Agent 开源项目精选

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

> 精心收集和分析优秀的 AI 智能体 (AI Agent) 相关开源软件，助力研究者和开发者快速了解领域前沿。

---

## 📋 目录

- [项目简介](#-项目简介)
- [AI Agent 框架](#-ai-agent-框架)
- [RAG 系统](#-rag-系统)
- [多智能体协调](#-多智能体协调)
- [工具与集成](#-工具与集成)
- [记忆系统](#-记忆系统)
- [分析与评估](#-分析与评估)
- [贡献指南](#-贡献指南)
- [许可证](#-许可证)

---

## 🎯 项目简介

本仓库旨在收集和系统分析 AI 智能体领域的高质量开源项目，涵盖：

- 🤖 **Agent 框架**: 构建智能体的基础架构
- 🧠 **RAG 系统**: 检索增强生成技术
- 🔄 **多智能体协调**: Multi-Agent 协作框架
- 🛠️ **工具集成**: Agent 工具调用生态
- 💾 **记忆系统**: 长期记忆与上下文管理
- 📊 **分析评估**: Agent 能力评测基准

每个项目都包含详细的架构分析、核心特性、使用场景和技术栈说明。

---

## 🤖 AI Agent 框架

### [MetaClaw](./analysis/MetaClaw/) ⭐ 3.5k+

**描述**: 元学习和进化的 AI Agent 框架 - 让 Agent 从每次对话中学习和进化

**核心特性**:
- 🦞 透明代理层设计，支持 OpenClaw/CoPaw/IronClaw/NanoClaw 等多种 Agent
- 🧬 基于 GRPO 算法的持续学习，无需 GPU 集群
- 📝 自动技能注入和总结
- 💾 跨会话长期记忆系统
- ⏰ 智能调度器（仅在空闲时训练）

**技术栈**: Python, FastAPI, PyTorch, LoRA, Tinker/MinT/Weaver

**使用场景**: 需要持续学习和进化的个人 AI 助手

**[查看详细分析 →](./analysis/MetaClaw/)**

---

### [OpenClaw](https://openclaw.ai) ⭐ 10k+

**描述**: 开源 AI 助手平台，支持多种渠道和工具集成

**核心特性**:
- 💬 多平台支持 (Discord, Telegram, Slack, 飞书等)
- 🔧 丰富的技能生态系统
- 🐳 容器化部署
- 🔒 安全沙箱执行

**技术栈**: TypeScript, Node.js, Docker

---

### [CoPaw](https://github.com/agentscope-ai/CoPaw)

**描述**: 多通道个人 Agent，支持多智能体协作

**核心特性**:
- 🎭 多角色 Agent 定义
- 🔗 Agent 间消息传递
- 📱 移动端支持

---

### [IronClaw](https://github.com/nearai/ironclaw)

**描述**: Rust 原生高性能个人 Agent

**核心特性**:
- ⚡ Rust 实现，高性能
- 🔧 丰富的工具集成
- 🛡️ 安全沙箱

**技术栈**: Rust

---

## 🧠 RAG 系统

### [RAGFlow](./analysis/RAGFlow/) ⭐ 20k+

**描述**: 基于深度文档理解的 RAG 引擎

**核心特性**:
- 📄 深度文档解析（PDF、Word、Excel 等）
- 🔍 多路召回策略
- 🎯 可解释的引用溯源
- 🏢 企业级部署支持

**技术栈**: Python, React, Elasticsearch

**[查看详细分析 →](./analysis/RAGFlow/)**

---

### [GraphRAG](./analysis/GraphRAG/) ⭐ 15k+

**描述**: 微软开源的基于知识图谱的 RAG 系统

**核心特性**:
- 🕸️ 自动构建知识图谱
- 🔗 图增强检索
- 📊 社区检测和摘要
- 🌍 全局查询支持

**技术栈**: Python, NetworkX, OpenAI

**[查看详细分析 →](./analysis/GraphRAG/)**

---

### [LightRAG](./analysis/LightRAG/)

**描述**: 轻量级 GraphRAG 实现

**核心特性**:
- ⚡ 低资源消耗
- 🔄 增量更新
- 🎯 精确检索

**[查看详细分析 →](./analysis/LightRAG/)**

---

### [Haystack](./analysis/Haystack/) ⭐ 10k+

**描述**: 端到端 NLP 框架，支持 RAG 和 Agent

**核心特性**:
- 🔧 模块化 Pipeline 设计
- 🤖 Agent 和工具支持
- 📦 多种文档存储后端
- 🧪 评估框架

**技术栈**: Python, Transformers

**[查看详细分析 →](./analysis/Haystack/)**

---

### [R2R](./analysis/R2R/)

**描述**: 快速、模块化的 RAG 框架

**核心特性**:
- 🔧 模块化架构
- 🚀 快速部署
- 📊 可观测性

**[查看详细分析 →](./analysis/R2R/)**

---

### [Verba](./analysis/Verba/)

**描述**: 基于 Weaviate 的 RAG 聊天机器人

**核心特性**:
- 🔍 Weaviate 向量数据库
- 💬 聊天界面
- 🔧 可配置检索策略

**[查看详细分析 →](./analysis/Verba/)**

---

### [AutoRAG](./analysis/AutoRAG/)

**描述**: RAG 评估和优化框架

**核心特性**:
- 📊 自动化评估
- 🔧 超参数优化
- 🎯 最佳实践推荐

**[查看详细分析 →](./analysis/AutoRAG/)**

---

### [Cognita](./analysis/Cognita/)

**描述**: 模块化生产级 RAG 框架

**核心特性**:
- 🏢 企业级部署
- 🔧 模块化组件
- 📊 可观测性

**[查看详细分析 →](./analysis/Cognita/)**

---

### [OpenRAG](./analysis/OpenRAG/)

**描述**: 综合 RAG 平台

**核心特性**:
- 🔧 多种检索策略
- 🤖 Agent 集成
- 📊 评估工具

**[查看详细分析 →](./analysis/OpenRAG/)**

---

### [RAG-Techniques](./analysis/RAG-Techniques/)

**描述**: RAG 技术实现示例集合

**核心特性**:
- 📚 多种 RAG 技术实现
- 🎯 最佳实践示例
- 🔧 可复用组件

**[查看详细分析 →](./analysis/RAG-Techniques/)**

---

### [Anything-LLM](./analysis/Anything-LLM/)

**描述**: 一体化 AI 生产力工具

**核心特性**:
- 💬 多工作区管理
- 📄 多文档类型支持
- 🔧 多模型支持

**[查看详细分析 →](./analysis/Anything-LLM/)**

---

### [Azure-Search-OpenAI-Demo](./analysis/Azure-Search-OpenAI-Demo/)

**描述**: Azure AI Search + OpenAI RAG 示例

**核心特性**:
- ☁️ Azure 云服务集成
- 🔍 Azure AI Search
- 🤖 OpenAI 集成

**[查看详细分析 →](./analysis/Azure-Search-OpenAI-Demo/)**

---

### [Langchain-Chatchat](./analysis/Langchain-Chatchat/)

**描述**: 基于 LangChain 的本地知识库问答

**核心特性**:
- 🏠 本地部署
- 📚 知识库管理
- 💬 多轮对话

**[查看详细分析 →](./analysis/Langchain-Chatchat/)**

---

### [Khoj](./analysis/Khoj/)

**描述**: 自托管 AI 第二大脑

**核心特性**:
- 🔍 个人知识搜索
- 💬 AI 对话
- 🏠 自托管

**[查看详细分析 →](./analysis/Khoj/)**

---

## 🔄 多智能体协调

### [AutoGen](https://github.com/microsoft/autogen) ⭐ 30k+

**描述**: 微软开源的多智能体对话框架

**核心特性**:
- 👥 多 Agent 对话编排
- 🔄 自动代码生成和执行
- 🛡️ 安全沙箱
- 🔧 可扩展的工具系统

**技术栈**: Python, OpenAI

---

### [CrewAI](https://github.com/joaomdmoura/crewai) ⭐ 20k+

**描述**: 角色扮演多智能体框架

**核心特性**:
- 🎭 角色定义和分配
- 🎯 任务委派和协调
- 🔄 顺序/并行执行
- 🛠️ 工具集成

**技术栈**: Python

---

### [MetaGPT](https://github.com/geekan/MetaGPT) ⭐ 40k+

**描述**: 多智能体协作软件开发框架

**核心特性**:
- 👔 模拟软件公司角色（产品经理、架构师、工程师等）
- 📝 自动生成需求文档、设计文档、代码
- 🔄 SOP 标准化流程

**技术栈**: Python

---

## 🛠️ 工具与集成

### [LangChain](./analysis/LangChain/) ⭐ 90k+

**描述**: LLM 应用开发框架

**核心特性**:
- 🔗 丰富的 LLM 和工具集成
- ⛓️ Chain 和 Agent 编排
- 💾 多种向量存储支持
- 🧪 评估和追踪

**技术栈**: Python, TypeScript

**[查看详细分析 →](./analysis/LangChain/)**

---

### [LlamaIndex](./analysis/LlamaIndex/) ⭐ 35k+

**描述**: LLM 数据框架

**核心特性**:
- 📄 数据连接器生态
- 🔍 高级检索策略
- 🤖 Agent 构建工具
- 📊 评估框架

**技术栈**: Python

**[查看详细分析 →](./analysis/LlamaIndex/)**

---

### [Quivr](./analysis/Quivr/)

**描述**: 第二大脑，知识管理 RAG 应用

**核心特性**:
- 🧠 知识库构建
- 💬 多模型对话
- 🔧 可扩展架构

**[查看详细分析 →](./analysis/Quivr/)**

---

### [Composio](https://github.com/composiohq/composio)

**描述**: AI Agent 工具集成平台

**核心特性**:
- 🔧 150+ 工具集成
- 🔐 托管认证
- 🎯 类型安全

---

## 💾 记忆系统

### [mem0](https://github.com/mem0ai/mem0) ⭐ 20k+

**描述**: 智能体长期记忆层

**核心特性**:
- 👤 用户级记忆
- 🧠 自适应记忆重要性
- 🔍 语义检索
- 🏢 多租户支持

**技术栈**: Python

---

### [mem0 + OpenClaw](https://github.com/mem0ai/mem0-openclaw)

**描述**: mem0 与 OpenClaw 的集成

---

## 📊 分析与评估

### [SWE-bench](https://github.com/princeton-nlp/SWE-bench)

**描述**: 软件工程 Agent 评测基准

**核心特性**:
- 🐛 真实 GitHub Issue 修复任务
- 📊 自动化评估
- 🔧 多语言支持

---

### [AgentBench](https://github.com/THUDM/AgentBench)

**描述**: 大语言模型 Agent 能力评测

**核心特性**:
- 🎮 多场景评测（OS、DB、Web、知识图谱等）
- 📊 综合评分体系

---

### [MetaClaw-Bench](https://github.com/aiming-lab/MetaClaw/tree/main/benchmark)

**描述**: AI Agent 多轮对话学习评测

**核心特性**:
- 📅 30 天完整数据集 / 12 天小型数据集
- 🔄 持续学习评估
- 📈 多维度指标

---

## 📈 项目统计

| 类别 | 项目数量 | 总 Stars |
|------|---------|---------|
| AI Agent 框架 | 4 | 13.5k+ |
| RAG 系统 | 14 | 45k+ |
| 多智能体协调 | 3 | 90k+ |
| 工具与集成 | 4 | 125k+ |
| 记忆系统 | 2 | 20k+ |
| 分析与评估 | 3 | - |

---

## 🤝 贡献指南

欢迎贡献！请遵循以下步骤：

1. **Fork** 本仓库
2. **创建目录**: 在 `analysis/` 目录下为每个项目创建独立目录
3. **添加分析**: 在目录中添加 README.md，包含架构分析、核心特性、使用场景
4. **更新主 README**: 在主 README 中添加项目链接（格式：`./analysis/项目名/`）
5. **提交 PR**: 使用清晰的标题和描述

### 目录结构模板

```
analysis/
└── project-name/
    └── README.md          # 项目详细分析
```

### 项目信息模板

```markdown
# 项目名称

**描述**: 一句话描述

## 核心特性
- 特性 1
- 特性 2
- 特性 3

## 技术栈
主要技术

## 使用场景
适用场景

## 架构分析
详细架构说明...

## 参考资料
- [GitHub 仓库](链接)
- [官方文档](链接)
```

---

## 📜 许可证

本项目采用 [MIT 许可证](LICENSE)。

所有收录的开源项目均遵循其各自的许可证条款。

---

## 🙏 致谢

感谢所有开源项目作者的贡献，推动了 AI Agent 领域的发展！

---

<div align="center">

**[⬆ 回到顶部](#awesome-research---ai-agent-开源项目精选)**

Made with ❤️ by [Raostu](https://github.com/Raostu)

</div>
