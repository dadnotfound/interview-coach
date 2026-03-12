# 贡献指南

感谢你对 interview-coach 项目的关注！我们欢迎任何形式的贡献。

## 🎯 如何贡献？

### 方式 1：新增场景 ⭐⭐⭐⭐⭐

**什么是场景？**
- 特定行业 + 特定岗位 + 特定轮次（初试/复试）
- 例如："金融 FinTech 初试 - 数据分析师"

**步骤：**
1. Fork 本仓库
2. 在 `assets/questions/` 创建新文件：
   ```
   scenario_004-fintech-data-analyst-initial.json
   ```
3. 添加 5-7 个问题
4. 提交 Pull Request

**场景文件格式：**
```json
{
  "id": "scenario_004",
  "name": "金融 FinTech 初试 - 数据分析师",
  "industry": "金融/FinTech",
  "role": "数据分析师",
  "stage": "初试",
  "difficulty": "L1",
  "questions": [
    {
      "id": "q001",
      "question": "请介绍一个你负责的数据分析项目",
      "goal": "项目经历",
      "hidden_problem": "项目参与度低"
    }
  ]
}
```

---

### 方式 2：改进现有问题

**什么样的改进是好改进？**
- 提高问题的开放性（更容易追问）
- 增加追问提示
- 优化问题的表达方式

**步骤：**
1. 找到需要改进的问题
2. 在 Issue 中提出改进建议
3. 等待审核通过后修改
4. 提交 Pull Request

---

### 方式 3：修复 Bug

**发现 Bug 了？**
- 请在 GitHub 上提交 Issue
- 详细描述问题
- 附带复现步骤
- 等待修复

---

### 方式 4：完善文档

- 📖 完善 README（使用说明、示例）
- 📖 补充 SKILL.md（核心框架）
- 📖 更新项目日志（记录进展）
- 📖 翻译成其他语言（英语、日语等）

---

### 方式 5：分享使用经验

- 📝 写博客文章介绍使用心得
- 🎥 发布视频教程
- 💬 在社区分享面试技巧
- 📊 在社交媒体展示进步曲线

---

## 📋 贡献规范

### ✅ 好的贡献应该：

1. **具体明确** - 不是泛泛而谈
2. **可量化** - 可以评估效果
3. **真实场景** - 来自真实面试
4. **行业相关** - 和岗位 JD 高度相关
5. **符合 STAR 原则** - 可以追问具体行为

### ❌ 不好的贡献：

1. **太泛泛** - "你有什么优势？"
2. **涉及隐私** - "你结婚了吗？"
3. **无法量化** - "你是一个有创意的人吗？"
4. **不相关** - "你平时喜欢做什么运动？"
5. **过于简单** - "你会用 Excel 吗？"

---

## 🔄 贡献流程

### Step 1：Fork 仓库
点击 GitHub 页面右上角的 "Fork" 按钮

### Step 2：Clone 仓库
```bash
git clone https://github.com/YOUR_USERNAME/interview-coach.git
cd interview-coach
```

### Step 3：创建分支
```bash
git checkout -b feature/your-feature-name
```

### Step 4：修改文件
按照上述规范修改文件

### Step 5：提交修改
```bash
git add .
git commit -m "Add: 新增 XXX 场景"
```

### Step 6：推送到 Fork
```bash
git push origin feature/your-feature-name
```

### Step 7：创建 Pull Request
访问 GitHub 页面，点击 "New Pull Request"

---

## 🎨 代码风格

### JSON 文件
- 使用 2 空格缩进
- 字段名用双引号
- 最后一项不加逗号

### Markdown 文件
- 使用标准 Markdown 语法
- 标题层级清晰
- 代码块标注语言

---

## 📝 Commit 消息规范

```
<类型>: <简短描述>

<详细描述>
```

**类型：**
- `Add`: 新增功能
- `Fix`: 修复 Bug
- `Update`: 更新文档
- `Optimize`: 优化代码
- `Refactor`: 重构代码

**示例：**
```
Add: 新增金融数据分析师场景

- 添加 5 个问题
- 添加 2 个隐藏问题
- 添加评估维度
```

---

## 🤝 代码审查

所有 Pull Request 都需要经过代码审查：

1. **自动检查** - CI/CD 自动检查格式
2. **人工审查** - 维护者审查内容
3. **测试验证** - 测试功能是否正常
4. **合并** - 通过后合并到主分支

---

## 📧 联系方式

- **GitHub Issues:** [提交问题](https://github.com/dadnotfound/interview-coach/issues)
- **邮箱:** 984525027@qq.com
- **Discord:** [加入社区](https://discord.gg/clawd)

---

## 🌟 贡献者

感谢所有贡献者！你的名字会出现在 [贡献者列表](CONTRIBUTORS.md) 中。

---

**开始贡献吧！** 🚀

_最后更新：2026-03-12_
