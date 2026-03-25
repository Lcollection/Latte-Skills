# 快速开始指南

## 1. 安装 Skills

### 方法 1: 使用 ClawHub (推荐)
```bash
# 安装所有 skills
cd D:\Latte-Skills\skills
for dir in */; do
  clawhub install "$dir"
done
```

### 方法 2: 手动复制
```bash
# 复制到 OpenClaw skills 目录
cp -r D:\Latte-Skills\skills\* D:\.openclaw\workspace\skills\
```

### 方法 3: 单个安装
```bash
# 只安装你需要的 skill
clawhub install paper-fetcher
clawhub install diagram-generator
```

## 2. 配置 API Keys

### Kimi API (用于翻译)
```bash
# 编辑配置文件
vim D:\PaperVault\config\translate.json
```

```json
{
  "provider": "kimi",
  "api_key": "sk-your-key-here",
  "base_url": "https://api.moonshot.cn/v1",
  "model": "moonshot-v1-8k",
  "enabled": true
}
```

### GLM API (可选)
```json
{
  "provider": "zai",
  "api_key": "your-glm-key",
  "base_url": "https://open.bigmodel.cn/api/paas/v4",
  "model": "glm-5"
}
```

## 3. 设置定时任务

### 使用 OpenClaw Cron
```bash
# 查看所有定时任务
/cron list

# 添加每日论文检索
/cron add "每日论文检索" "0 8 * * *" "运行论文检索"

# 添加每日总结
/cron add "每日学习总结" "0 20 * * *" "生成每日总结"
```

### 手动配置
编辑 `D:\PaperVault\config\cron.json`:
```json
{
  "jobs": [
    {
      "name": "每日论文检索",
      "schedule": "0 8 * * *",
      "script": "daily-search.py",
      "enabled": true
    }
  ]
}
```

## 4. 开始使用

### 论文检索
```
"搜索今天的论文"
"检索 arXiv 上关于 transformer 的最新论文"
```

### 学习报告
```
"生成今天的每日总结"
"生成本周学习周报"
```

### 图表生成
```
"画一个用户登录的流程图"
"生成一个系统架构图"
```

### 演示文稿
```
"创建一个关于机器学习的 Slidev 演示"
```

## 5. 验证安装

### 检查 Skills
```bash
# 列出所有已安装的 skills
ls D:\.openclaw\workspace\skills
```

### 测试运行
```bash
# 测试论文检索
python D:\PaperVault\scripts\daily-search.py

# 测试总结生成
python D:\PaperVault\scripts\daily-summary.py
```

## 6. 常见问题

### Q: Skills 不生效？
A: 检查 OpenClaw 配置，确保 skills 目录正确

### Q: 翻译失败？
A: 检查 API key 是否正确，检查配额是否用完

### Q: Zotero 导入失败？
A: 确保 Zotero 正在运行，Connector 已启用

### Q: 定时任务不运行？
A: 检查 cron 配置，确保 enabled 为 true

## 7. 进阶配置

### 自定义关键词
编辑 `D:\PaperVault\config\keywords.json`:
```json
{
  "keywords": [
    "your research field",
    "your interests"
  ],
  "max_papers_per_day": 20
}
```

### 自定义模板
修改 `D:\PaperVault\templates\` 目录下的模板文件

### 集成 Obsidian
将 `D:\PaperVault` 设为 Obsidian vault

## 8. 更新 Skills

```bash
# 拉取最新版本
cd D:\Latte-Skills
git pull

# 重新安装
clawhub install --force
```

## 9. 获取帮助

- 📖 查看文档: `D:\Latte-Skills\docs\`
- 💬 提交问题: [GitHub Issues](https://github.com/Lcollection/Latte-Skills/issues)
- 📧 联系作者: your@email.com

---

[← 返回主页](../README.md)
