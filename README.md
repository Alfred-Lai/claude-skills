# Claude Code Skills 合集

个人 Claude Code Skills 仓库，用于集中管理和版本控制自定义 skill。

## 已有 Skills

### 1. credit-review-report — 银行授信审查报告撰写

基于兴业银行真实审查报告模板，帮助银行信贷审查员在获取企业信息（企业介绍、财务报表、企查查报告等）后，生成专业的授信审查报告。

**支持产品类型：**
- 传统授信（流贷 / 银承 / 信用证 / 保函）
- 项目贷款 / 房地产开发贷款
- 定增融资 / 股票收益权
- 集团授信

**支持业务场景：** 首笔新增、续作维持、续作压缩、存量扩盘

**核心能力：**
- 强制关键信息确认环节（7 项必确认 + 3 项条件确认）
- 深度行业分析（"三贴合"原则：贴合细分赛道、区域产业、上下游景气度）
- 四期财务对比分析（含科目明细和异动分析）
- 九段式标准报告结构
- 自动生成 Word 文档（.docx），严格遵循中文公文排版规范

## 安装方式

将 skill 目录复制到你的 Claude Code 项目的 `.claude/skills/` 下：

```bash
# 克隆仓库
git clone https://github.com/zinovy/claude-skills.git

# 复制需要的 skill
cp -r claude-skills/skills/credit-review-report /你的项目路径/.claude/skills/
```

## 目录结构

```
claude-skills/
├── README.md
└── skills/
    └── credit-review-report/
        ├── SKILL.md                          # 主 skill 定义
        └── references/                       # 参考指南
            ├── financial-analysis-guide.md   # 财务分析深度指南
            ├── industry-search-guide.md      # 行业联网搜索策略
            └── product-templates.md          # 四种产品类型差异化模板
```

## 更新日志

- **2026-05-30** — 初始化仓库，添加 `credit-review-report` skill
