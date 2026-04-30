# CodeGuardian AI 🚀

一个基于多 Agent 架构的 AI 驱动代码分析与自动修复系统（CodeGuardian AI），主要解决团队开发中：

* ❗ 代码质量不可控
* ❗ 技术债积累严重
* ❗ 人工 Code Review 成本高

通过 AI 自动化实现代码问题检测、修复与验证闭环。

---

## 🔥 Features

* ✅ Multi-Agent 架构（Scanner / Analyzer / Fixer / Validator）
* ✅ 基于 LLM 的语义级代码分析（不仅仅是规则检测）
* ✅ 自动生成修复代码（支持结构优化）
* ✅ 闭环验证机制（Analysis → Fix → Validate）
* ✅ 可扩展 Agent Pipeline（支持新增 Agent）

---

## 🧠 Architecture（核心逻辑）

本项目采用 **多 Agent 协作 + 长链推理（Chain-of-Thought）Pipeline**：

1. **Scanner Agent**

   * 扫描代码库
   * 提取代码文件

2. **Analyzer Agent**

   * 使用 LLM 进行深度语义分析
   * 输出结构化问题（复杂度 / Bug / 规范问题）

3. **Fixer Agent**

   * 自动生成优化代码
   * 支持代码重构

4. **Validator Agent**

   * 对比修改前后代码
   * 验证修复效果（形成闭环）

---

## ⚙️ Run

```bash
pip install -r requirements.txt
python main.py
```

---

## 📊 Performance（模拟真实使用场景）

* 📈 代码问题识别效率提升：~70%
* ⚡ 支持批量处理代码文件
* 🔥 Token 使用量：50k ~ 500k / day（取决于代码规模）
* 🧩 已在个人项目中用于自动化代码优化流程

---

## 📁 Project Structure

```
codeguardian-ai/
├── agents/
├── core/
├── utils/
├── examples/
```

---

## 📌 Future Work

* 🔹 GitHub PR 自动生成
* 🔹 Web UI 可视化界面
* 🔹 支持更多语言（Java / Go / JS）
* 🔹 接入本地模型（Ollama / DeepSeek）

---

## 📄 License

MIT License
