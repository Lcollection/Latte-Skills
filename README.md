# Latte Skills ☕

> OpenClaw Agent Skills Collection

[![OpenClaw](https://img.shields.io/badge/OpenClaw-Compatible-brightgreen)](https://openclaw.ai)
[![Skills](https://img.shields.io/badge/Skills-9-blue)](./skills)
[![License](https://img.shields.io/badge/License-MIT-green)](./LICENSE)

---

## 📦 Skills 列表

### 📚 论文与学习

| Skill | 功能 | 状态 |
|-------|------|------|
| [**Paper Fetcher**](./skills/paper-fetcher) | arXiv 论文自动检索、翻译、导入 | ✅ 稳定 |
| [**Paper Summarizer**](./skills/paper-summarizer) | 生成每日/每周/月度学习报告 | ✅ 稳定 |
| [**Learning Reflector**](./skills/learning-reflector) | 深度反思学习，发现盲点 | ✅ 稳定 |
| [**PDF Reader**](./skills/pdf-reader) | PDF 深度阅读和分析 | ✅ 稳定 |
| [**PaperVault Cron**](./skills/papervault-cron) | 完整论文自动化工作流 | ✅ 稳定 |

### 🛠️ 工具与效率

| Skill | 功能 | 状态 |
|-------|------|------|
| [**Token Usage Tracker**](./skills/token-usage-tracker) | 追踪 API Token 消耗 | ✅ 稳定 |
| [**Diagram Generator**](./skills/diagram-generator) | 生成流程图、时序图等 | ✅ 稳定 |
| [**Slidev Generator**](./skills/slidev-generator) | 自动生成 Slidev 演示文稿 | ✅ 稳定 |
| [**GitHub CLI**](./skills/github-cli) | GitHub 自动化操作 | ✅ 稳定 |

---

## 🚀 快速开始

### 1. 克隆仓库

```bash
git clone https://github.com/Lcollection/Latte-Skills.git
cd Latte-Skills
```

### 2. 安装 Skill

#### 方法 1: 手动安装
```bash
# 复制到你的 OpenClaw skills 目录
cp -r skills/* ~/.openclaw/skills/
```

#### 方法 2: 使用 ClawHub (推荐)
```bash
# 从 ClawHub 安装
npx clawhub@latest install <skill-name>
```

### 3. 使用 Skill

在 OpenClaw 中直接触发：

```
搜索今天的论文          # Paper Fetcher
生成学习总结            # Paper Summarizer
画一个流程图            # Diagram Generator
创建一个演示文稿        # Slidev Generator
```

---

## 🎨 特色功能

### 1. 自动化论文工作流

```mermaid
graph LR
    A[arXiv 检索] --> B[自动翻译]
    B --> C[导入 Zotero]
    C --> D[生成笔记]
    D --> E[学习总结]
    E --> F[反思优化]
    
    style A fill:#4caf50,color:#fff
    style F fill:#2196f3,color:#fff
```

### 2. 智能图表生成

支持 10+ 种图表类型：
- 流程图 (Flowchart)
- 时序图 (Sequence Diagram)
- 类图 (Class Diagram)
- ER 图 (ER Diagram)
- 甘特图 (Gantt Chart)
- 状态图 (State Diagram)
- 饼图 (Pie Chart)
- 思维导图 (Mind Map)

### 3. Token 使用追踪

实时监控 API 消耗：
- 每日/每周/每月统计
- 成本计算
- 配额警告
- 使用趋势分析

---

## 💡 使用场景

### 科研工作者
```
"搜索今天的机器学习论文"        → Paper Fetcher
"生成本周学习周报"              → Paper Summarizer
"反思我的学习盲点"              → Learning Reflector
```

### 技术分享
```
"画一个微服务架构图"            → Diagram Generator
"创建一个技术分享演示"          → Slidev Generator
"导出为 PDF"                    → Slidev Generator
```

### 成本管理
```
"查看今天的 token 使用量"       → Token Usage Tracker
"生成本月成本报告"              → Token Usage Tracker
```

---

## 📊 Skill 对比

| Skill | 自动化 | LLM 支持 | 图表支持 | 导出格式 |
|-------|--------|---------|---------|---------|
| Paper Fetcher | ✅ | ✅ | - | Markdown |
| Paper Summarizer | ✅ | - | - | Markdown |
| Learning Reflector | - | ✅ | ✅ | Markdown |
| PDF Reader | - | ✅ | - | Markdown |
| Token Tracker | ✅ | - | ✅ | JSON/MD |
| Diagram Generator | - | ✅ | ✅ | Mermaid |
| Slidev Generator | - | ✅ | ✅ | PDF/PNG/SPA |
| GitHub CLI | ✅ | - | - | - |
| PaperVault Cron | ✅ | ✅ | - | Markdown |

---

## 📝 更新日志

### v1.0.0 (2026-03-25)

**首次发布**
- ✨ Paper Fetcher - 论文检索与导入
- ✨ Paper Summarizer - 学习报告生成
- ✨ Learning Reflector - 学习反思与优化
- ✨ PDF Reader - PDF 深度阅读
- ✨ Token Usage Tracker - API Token 追踪
- ✨ Diagram Generator - 流程图生成
- ✨ Slidev Generator - 演示文稿生成
- ✨ GitHub CLI - GitHub 自动化操作
- ✨ PaperVault Cron - 完整工作流

---

## 📄 许可证

本项目采用 MIT 许可证 - 查看 [LICENSE](./LICENSE) 文件了解详情
