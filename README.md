# Latte Skills ☕

> OpenClaw Agent Skills Collection - 提升你的 AI 助手能力

[![OpenClaw](https://img.shields.io/badge/OpenClaw-Compatible-brightgreen)](https://openclaw.ai)
[![Skills](https://img.shields.io/badge/Skills-8-blue)](./skills)
[![License](https://img.shields.io/badge/License-MIT-green)](./LICENSE)

## 🎯 简介

Latte Skills 是一组为 OpenClaw Agent 设计的技能包，涵盖论文管理、学习辅助、图表生成、演示制作等多个领域。

**为什么叫 Latte？**
- ☕ 像 Latte 一样，为你的 AI 助手增添风味
- 🚀 简单易用，即插即用
- 🎨 优雅设计，功能强大

---

## 📦 Skills 列表

### 📚 论文与学习

| Skill | 功能 | 状态 |
|-------|------|------|
| [**Paper Fetcher**](./skills/paper-fetcher) | arXiv 论文自动检索、翻译、导入 | ✅ 稳定 |
| [**Paper Summarizer**](./skills/paper-summarizer) | 生成每日/每周/月度学习报告 | ✅ 稳定 |
| [**Learning Reflector**](./skills/learning-reflector) | 深度反思学习，发现盲点 | ✅ 稳定 |
| [**PDF Reader**](./skills/pdf-reader) | PDF 深度阅读和分析 | ✅ 稳定 |
| [**GitHub CLI**](./skills/github-cli) | GitHub 自动化操作 | ✅ 稳定 |
| [**PaperVault Cron**](./skills/papervault-cron) | 完整论文自动化工作流 | ✅ 稳定 |

### 🛠️ 工具与效率

| Skill | 功能 | 状态 |
|-------|------|------|
| [**Token Usage Tracker**](./skills/token-usage-tracker) | 追踪 API Token 消耗 | ✅ 稳定 |
| [**Diagram Generator**](./skills/diagram-generator) | 生成流程图、时序图等 | ✅ 稳定 |
| [**Slidev Generator**](./skills/slidev-generator) | 自动生成 Slidev 演示文稿 | ✅ 稳定 |

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

## 📖 详细文档

### 核心功能

- [Paper Fetcher 使用指南](./docs/paper-fetcher-guide.md)
- [Paper Summarizer 使用指南](./docs/paper-summarizer-guide.md)
- [Diagram Generator 示例](./docs/diagram-examples.md)
- [Slidev Generator 教程](./docs/slidev-tutorial.md)

### 配置与部署

- [配置文件说明](./docs/configuration.md)
- [定时任务设置](./docs/cron-setup.md)
- [API 密钥配置](./docs/api-keys.md)

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

---

## 🤝 贡献指南

欢迎贡献新的 skill 或改进现有 skill！

### 如何贡献

1. Fork 本仓库
2. 创建你的 feature 分支 (`git checkout -b feature/AmazingSkill`)
3. 提交更改 (`git commit -m 'Add some AmazingSkill'`)
4. 推送到分支 (`git push origin feature/AmazingSkill`)
5. 创建 Pull Request

### Skill 开发规范

每个 skill 应包含：
- ✅ `SKILL.md` - Skill 主文档
- ✅ `README.md` - 使用说明
- ✅ `config/` - 配置文件（如需要）
- ✅ `scripts/` - 脚本文件（如需要）
- ✅ `examples/` - 使用示例

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
- ✨ PaperVault Cron - 完整工作流

---

## 📄 许可证

本项目采用 MIT 许可证 - 查看 [LICENSE](./LICENSE) 文件了解详情

---

## 🙏 致谢

- [OpenClaw](https://openclaw.ai) - 强大的 AI Agent 平台
- [ClawHub](https://clawhub.com) - Skills 分享平台
- [Mermaid](https://mermaid.js.org/) - 图表生成库
- [Slidev](https://sli.dev/) - 演示文稿工具

---

## 📞 联系方式

- **作者**: Echo (OpenClaw Assistant)
- **维护者**: 李修旭 (Ethan)
- **GitHub**: [Lcollection](https://github.com/Lcollection)
- **Issues**: [提交问题](https://github.com/Lcollection/Latte-Skills/issues)

---

<div align="center">

**[⬆ 返回顶部](#latte-skills-)**

Made with ☕ by Echo

</div>
