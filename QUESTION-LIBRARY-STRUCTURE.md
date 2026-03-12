# 面试题库结构规范（开源共建版）

**目标：** 建立一个可扩展、标准化的面试题库，支持社区共建

---

## 📁 目录结构

```
interview-coach-skill/
├── assets/questions/
│   ├── README.md                    # 贡献指南
│   ├── SCHEMA.md                    # 题库格式规范
│   ├── .github/                     # GitHub 模板
│   │   ├── ISSUE_TEMPLATE/          # Issue 模板
│   │   │   ├── new-question.md      # 提交新问题
│   │   │   ├── bug-report.md        # Bug 报告
│   │   │   └── improvement.md       # 改进建议
│   │   └── PULL_REQUEST_TEMPLATE.md # PR 模板
│   ├── tech/                        # 互联网/科技
│   │   ├── product-manager.json
│   │   ├── engineer.json
│   │   └── operations.json
│   ├── fintech/                     # 金融/FinTech
│   │   ├── analyst.json
│   │   ├── risk-control.json
│   │   └── product-manager.json
│   ├── ev/                          # 新能源/车企
│   │   ├── algorithm-engineer.json
│   │   ├── battery-expert.json
│   │   └── product-manager.json
│   ├── health/                      # 医疗健康
│   │   ├── product-manager.json
│   │   ├── operations.json
│   │   └── sales.json
│   └── ai/                          # 智能制造/AI
│       ├── scientist.json
│       ├── data-scientist.json
│       └── product-manager.json
└── .metadata/                       # 元数据
    ├── contributors.json             # 贡献者列表
    ├── changelog.md                 # 变更日志
    └── stats.json                   # 统计信息
```

---

## 📋 SCHEMA.md - 题库格式规范

### 题库文件格式（JSON）

```json
{
  "meta": {
    "version": "1.0.0",
    "industry": "互联网/科技",
    "role": "产品经理",
    "last_updated": "2026-03-11",
    "contributors": ["openclaw", "community"],
    "total_questions": 50
  },
  "questions": [
    {
      "id": "tech-pm-001",
      "question": "请介绍一个你负责的产品项目",
      "category": "项目经验",
      "difficulty": "L2",
      "tags": ["STAR", "追问", "产品思维"],
      "scenario": "产品经理初试",
      "triggers_hidden_issue": true,
      "hidden_issue_type": "过度包装",
      "follow_up_questions": [
        "具体是什么场景？",
        "你的角色是什么？",
        "你做了什么？",
        "结果如何？"
      ],
      "expected_answer_points": [
        "项目背景和目标",
        "个人角色和贡献",
        "遇到的挑战",
        "解决方案和结果"
      ],
      "red_flags": [
        "回答模糊，无具体细节",
        "夸大个人贡献",
        "无法量化结果"
      ],
      "source": "原创/社区贡献",
      "contributor": "openclaw",
      "created_at": "2026-03-11",
      "verified": true
    }
  ]
}
```

### 字段说明

| 字段 | 类型 | 必填 | 说明 |
|------|------|------|------|
| `id` | string | ✅ | 唯一标识符，格式：`{industry}-{role}-{number}` |
| `question` | string | ✅ | 问题内容 |
| `category` | string | ✅ | 问题分类（项目经验/技能/软技能等） |
| `difficulty` | string | ✅ | 难度等级（L1-L4） |
| `tags` | array | ✅ | 标签（STAR/追问/产品思维等） |
| `scenario` | string | ⚠️ | 适用场景（产品经理初试/复试等） |
| `triggers_hidden_issue` | boolean | ❌ | 是否触发隐藏问题 |
| `hidden_issue_type` | string | ❌ | 隐藏问题类型 |
| `follow_up_questions` | array | ❌ | 追问示例 |
| `expected_answer_points` | array | ❌ | 期望回答要点 |
| `red_flags` | array | ❌ | 警告信号 |
| `source` | string | ❌ | 来源（原创/社区贡献/引用） |
| `contributor` | string | ❌ | 贡献者 |
| `created_at` | string | ❌ | 创建时间 |
| `verified` | boolean | ❌ | 是否已验证 |

---

## 🤝 贡献指南（README.md）

### 如何贡献？

#### 方式 1：提交新问题

1. **Fork 本仓库**
2. **创建分支**：`git checkout -b add-new-question`
3. **添加问题**：在对应的 JSON 文件中添加问题
4. **提交 PR**：`git commit -m "Add: 新增产品经理面试题"`
5. **创建 Pull Request**

#### 方式 2：提交 Issue

如果你不熟悉 Git，也可以通过 Issue 提交：
1. 点击 "New Issue"
2. 选择 "提交新问题" 模板
3. 填写表单
4. 提交

#### 方式 3：改进现有问题

1. 找到需要改进的问题
2. 提出改进建议（通过 Issue 或 PR）
3. 等待审核

---

### 贡献规范

#### ✅ 好的问题应该：

1. **具体明确** - 不是泛泛而谈
2. **可量化** - 可以评估回答质量
3. **真实场景** - 来自真实面试
4. **行业相关** - 和岗位 JD 高度相关
5. **符合 STAR** - 可以追问具体行为

#### ❌ 不好的问题：

1. **太泛泛** - "你有什么优势？"
2. **涉及隐私** - "你结婚了吗？"
3. **无法量化** - "你是一个有创意的人吗？"
4. **不相关** - "你平时喜欢做什么运动？"
5. **过于简单** - "你会用 Excel 吗？"

---

### 审核标准

所有贡献都会经过审核，确保：
1. **格式正确** - 符合 SCHEMA.md 规范
2. **质量合格** - 问题有价值、有深度
3. **无重复** - 和现有问题不重复
4. **合规** - 不涉及隐私和歧视
5. **专业** - 符合行业标准

---

## 📊 社区共建激励

### 贡献者等级

| 等级 | 贡献次数 | 权限 |
|------|---------|------|
| **观察者** | 0 | 只能查看 |
| **贡献者** | 1-10 次 | 可提交问题 |
| **审核者** | 11-50 次 | 可审核 PR |
| **维护者** | 50+ 次 | 可合并 PR |

### 贡献统计

所有贡献者都会在 `contributors.json` 中记录：
```json
{
  "contributors": [
    {
      "username": "openclaw",
      "contributions": 50,
      "role": "maintainer",
      "bio": "项目发起人"
    },
    {
      "username": "community-member-1",
      "contributions": 5,
      "role": "contributor",
      "bio": "产品经理，5 年经验"
    }
  ]
}
```

---

## 🎯 下一步行动

### 立即执行

1. **创建题库目录结构**
2. **编写 SCHEMA.md**
3. **编写贡献指南 README.md**
4. **创建 GitHub Issue 和 PR 模板**
5. **手动补充 AI 行业题库**

### 发布准备

1. **推送到 GitHub**
2. **编写 README.md（项目介绍）**
3. **设置 GitHub Pages（文档网站）**
4. **发布到 ClawHub**

---

**目标：** 建立一个可持续、可扩展的开源面试题库，邀请全球开发者共建！

_最后更新：2026-03-11_