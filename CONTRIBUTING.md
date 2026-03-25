# Contributing to Latte Skills

感谢你考虑为 Latte Skills 做贡献！🎉

## 🤔 如何贡献

### 报告 Bug
1. 检查 [Issues](https://github.com/Lcollection/Latte-Skills/issues) 中是否已有相同问题
2. 如果没有，创建新 Issue，包含：
   - 清晰的标题
   - 详细的描述
   - 复现步骤
   - 预期行为 vs 实际行为
   - 环境信息（OS, Node.js 版本等）

### 提出新功能
1. 创建 Issue 描述你的想法
2. 说明为什么这个功能有用
3. 提供可能的实现方案

### 提交代码

#### 1. Fork & Clone
```bash
git clone https://github.com/YOUR_USERNAME/Latte-Skills.git
cd Latte-Skills
```

#### 2. 创建分支
```bash
git checkout -b feature/your-feature-name
```

#### 3. 进行修改
- 遵循现有的代码风格
- 添加必要的注释
- 更新相关文档

#### 4. 测试
确保你的修改不会破坏现有功能

#### 5. 提交
```bash
git add .
git commit -m "feat: add some amazing feature"
```

提交信息格式：
- `feat:` 新功能
- `fix:` Bug 修复
- `docs:` 文档更新
- `style:` 代码格式
- `refactor:` 重构
- `test:` 测试相关
- `chore:` 构建/工具相关

#### 6. 推送
```bash
git push origin feature/your-feature-name
```

#### 7. 创建 Pull Request
- 清晰描述你的修改
- 关联相关的 Issue
- 等待审核

## 📋 Skill 开发规范

### 目录结构
```
skill-name/
├── SKILL.md              # Skill 主文档（必需）
├── README.md             # 使用说明（必需）
├── config/               # 配置文件
│   └── default.json
├── scripts/              # 脚本文件
│   └── main.py
├── templates/            # 模板文件
│   └── example.md
└── examples/             # 使用示例
    └── demo.md
```

### SKILL.md 规范
```yaml
---
name: Skill Name
slug: skill-name
version: 1.0.0
description: "简短描述"
---

## When to Use
触发条件和使用场景

## Quick Start
快速开始指南

## Features
功能列表

## Configuration
配置说明
```

### 代码规范
- Python: 遵循 PEP 8
- JavaScript: 使用 ESLint
- 添加类型提示（Python 3.8+）
- 编写清晰的注释

### 文档规范
- 使用 Markdown 格式
- 包含代码示例
- 添加必要的图表
- 保持简洁明了

## 🧪 测试

### 手动测试
```bash
# 测试 skill
python scripts/test-skill.py --skill paper-fetcher
```

### 自动化测试
```bash
# 运行所有测试
npm test
```

## 📚 资源

- [OpenClaw 文档](https://docs.openclaw.ai)
- [ClawHub 平台](https://clawhub.com)
- [Skill 开发指南](https://docs.openclaw.ai/skills)

## 💬 获取帮助

- 💬 [Discord 社区](https://discord.gg/clawd)
- 📧 邮件: your@email.com
- 📖 [文档](https://github.com/Lcollection/Latte-Skills/tree/main/docs)

## 📜 行为准则

- 尊重所有贡献者
- 保持友好和建设性的讨论
- 接受建设性批评
- 关注对社区最有利的事情

## ✅ 检查清单

提交 PR 前确保：
- [ ] 代码遵循项目规范
- [ ] 添加了必要的文档
- [ ] 测试通过
- [ ] 提交信息清晰
- [ ] 关联了相关 Issue

---

再次感谢你的贡献！❤️
