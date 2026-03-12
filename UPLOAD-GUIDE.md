# GitHub 手动上传操作指南

**时间：** 2026-03-12 20:40 GMT+8
**目标：** 将本地文件手动上传到 GitHub

---

## 📋 **需要上传的文件（按优先级）**

### P0：必须上传（核心文件）
1. `LICENSE` - MIT License
2. `README.md` - 项目说明（8860 字）
3. `CONTRIBUTING.md` - 贡献指南
4. `CHANGELOG.md` - 版本日志
5. `CODE_OF_CONDUCT.md` - 行为准则
6. `ISSUE_TEMPLATE.md` - Issue 模板
7. `BUG_REPORT.md` - Bug 报告模板
8. `PROGRESS-REPORT.md` - 进度报告

### P1：建议上传（补充文件）
9. 所有 `assets/questions/` 目录下的 JSON 文件
10. 所有 `references/` 目录下的 Markdown 文件

---

## 🚀 **快速操作步骤**

### **Step 1：访问 GitHub 仓库**
```
https://github.com/dadnotfound/interview-coach
```

### **Step 2：上传 LICENSE**
1. 点击 "Add file" → "Create new file"
2. 文件名：`LICENSE`
3. 内容：复制以下内容

```text
MIT License

Copyright (c) 2026 赵浩

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
```

4. 提交说明：`Add MIT License`
5. 点击 "Commit new file"

---

### **Step 3：上传 README.md**
1. 点击 "Add file" → "Create new file"
2. 文件名：`README.md`（覆盖现有文件）
3. 内容：访问本地文件
   ```
   /root/.openclaw/workspace/interview-coach-temp/README.md
   ```
4. 复制完整内容（8860 字）
5. 提交说明：`Update README - 完善版（8860 字）`
6. 点击 "Commit new file"

---

### **Step 4：上传其他文档**
重复 Step 3 的操作，上传以下文件：

1. `CONTRIBUTING.md`
2. `CHANGELOG.md`
3. `CODE_OF_CONDUCT.md`
4. `ISSUE_TEMPLATE.md`
5. `BUG_REPORT.md`
6. `PROGRESS-REPORT.md`

**提示：** 这些文件内容我已准备好，你可以访问本地路径复制：
```
/root/.openclaw/workspace/interview-coach-temp/
```

---

### **Step 5：验证上传**
上传完成后，访问以下链接验证：

1. **LICENSE：**
   ```
   https://raw.githubusercontent.com/dadnotfound/interview-coach/main/LICENSE
   ```
   应该看到 MIT License 内容

2. **README.md：**
   ```
   https://raw.githubusercontent.com/dadnotfound/interview-coach/main/README.md
   ```
   应该看到新的 README 内容（包含 "开源共建" 等字样）

3. **CONTRIBUTING.md：**
   ```
   https://raw.githubusercontent.com/dadnotfound/interview-coach/main/CONTRIBUTING.md
   ```
   应该看到贡献指南

---

## 📝 **GitHub 仓库设置优化**

上传完文件后，还需要优化仓库设置：

### **1. 添加 Topics**
1. 访问：https://github.com/dadnotfound/interview-coach
2. 点击右上角的 "⚙️ Settings"
3. 滚动到 "Topics" 部分
4. 添加以下标签：
   - `interview`
   - `hr`
   - `ai`
   - `openclaw`
   - `coaching`
   - `recruitment`
   - `talent`

### **2. 添加 Description**
在 "Description" 字段填写：
```
AI 面试官培训工具 - 通过模拟真实面试场景中的"隐藏问题"，帮助面试官提升追问技巧、洞察能力和控场能力
```

### **3. 添加 Homepage**
如果将来有 ClawHub 链接，填写到 "Website" 字段

### **4. 设置 License**
1. 滚动到 "License" 部分
2. 选择 "MIT License"
3. 点击 "Save changes"

---

## ⏰ **预计耗时**

- **Step 2-3：** 10-15 分钟（上传 LICENSE + README）
- **Step 4：** 10-15 分钟（上传其他文档）
- **Step 5：** 5 分钟（验证）
- **GitHub 设置：** 5 分钟

**总计：** 30-40 分钟

---

## ✅ **完成标准**

- [ ] LICENSE 已上传
- [ ] README.md 已更新
- [ ] 所有文档已上传
- [ ] Topics 已添加
- [ ] Description 已添加
- [ ] License 已设置

---

## 🎯 **完成后**

完成后，告诉我：
1. 哪些文件已上传
2. 哪些设置已优化
3. 是否遇到问题

然后我会：
1. 验证上传结果
2. 检查仓库状态
3. 准备 Phase 4（明早执行）

---

**准备好开始了吗？** 🚀

_操作指南：虾球（AI 助手）_
_时间：2026-03-12 20:40 GMT+8_
