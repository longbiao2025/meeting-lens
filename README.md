
# Meeting-Lens

**通用会议纪要萃取引擎** 采用自适应动态切片 + 子代理并行处理技术，从**关键事实、难点聚焦、核心结论、任务部署**四个维度深度萃取长文本会议精华。

---

## ✨ 核心亮点

- **防偷懒设计**：严格禁止大模型一次性通读长文本提取具体任务细节
- **自适应动态切片**：智能均分 + 重叠视窗，确保长会议不遗漏、不割裂
- **子代理并行处理**：基于全局上下文指纹的多代理深度采掘
- **五维分类法**：客观事实、问题分析、核心结论、任务部署 + 角色动态推演
- **专业化输出**：输出高质量、可直接使用的正式会议纪要（Markdown + Word）
- **严格纯净输出**：仅输出正式纪要，绝无任何废话和解释

---

## 📋 Skill 信息

- **名称**：meeting-lens
- **版本**：1.0
- **作者**：高龙彪
- **许可证**：Apache-2.0
- **适用场景**：长达数万字的会议转写文本、项目复盘会、业务分析会、战略研讨会等

---

## 🚀 使用方法

### 1. 准备工作
将需要处理的会议原始转写文本保存为 `.txt` 或 `.md` 文件（推荐 UTF-8 编码）。

### 2. 调用 Skill
在支持该 skill 的平台（如 Claude、Cursor 等）中，使用以下方式调用：

```markdown
使用 meeting-lens skill 处理以下会议纪要：

[在此粘贴或上传完整的会议转写文本]
````

### 3\. 输出要求

  - 最终输出为纯 Markdown 格式的正式会议纪要
  - 自动生成结构化的 Word 文档（含专业排版）
  - 输出语言与原始会议文档语言保持一致（默认中文）

-----

## 📘 输出结构（示例）

**【会议标题】会议纪要**

**一、会议背景与核心议题**
（约300字，包含会议动机、核心目标、参会关键角色）

**二、关键事实与信息通报**
（详实的数据、进度、指标、案例）

**三、问题分析与难点聚焦**
（业务痛点、认知分歧、核心矛盾）

**四、核心结论与管理要求**
（领导拍板决策、管理红线及决策依据）

**五、任务部署与责任矩阵**

| 责任人 | 动作指令 | 交付标准 | 资源依赖 | 截止时间 |
| :--- | :--- | :--- | :--- | :--- |
| [姓名/角色] | [清晰的行动指令] | [具体的交付成果] | [需要的支持/资源] | [YYYY-MM-DD] |

-----

## 🛠️ 技术实现亮点

1.  **第1步**：全量速读提取全局上下文指纹
2.  **第2步**：自适应动态切片（4000-5000字基准 + 500字重叠）
3.  **第3步**：子代理并行执行五维深度萃取
4.  **第4-5步**：二次自检 + 全局缝合去重
5.  **第6步**：标准化 Markdown 渲染
6.  **第7步**：导出专业排版 Word 文档（宋体 + 小四）
7.  **第8步**：自动清理临时文件

-----

## 📄 许可证

本项目采用 Apache License 2.0 开源协议。

## 👤 作者

**高龙彪**
GitHub: [@gaolongbiao](https://www.google.com/search?q=https://github.com/gaolongbiao)

## ⭐ Star 支持

如果你觉得 Meeting-Lens 对你的会议效率提升有帮助，欢迎给这个项目点个 Star！
欢迎提交 Issue 和 Pull Request，一起把会议纪要萃取做得更好！

## 📬 联系与反馈

  - **GitHub Issues**：欢迎提出使用中的任何问题或改进建议
  - **作者 X (Twitter)**：@gaolongbiao

> 让每一场会议的精华，都不被浪费。
> **Meeting-Lens — 让长会议也有清晰的骨骼与灵魂。**

-----

-----

# Meeting-Lens

**Universal Meeting Summary Extraction Engine**
An intelligent meeting minutes distillation system that uses **adaptive dynamic chunking** and **sub-agent parallel processing** to deeply extract the essence of long meeting transcripts from four key dimensions: **Key Facts, Problem Analysis, Core Conclusions, and Task Deployment**.

-----

## ✨ Key Features

  - **Anti-Laziness Design**: Strictly prohibits large language models from performing one-shot summarization on long texts when extracting specific action items and details.
  - **Adaptive Dynamic Chunking**: Intelligently splits text with balanced chunk sizes and 500-character overlap to prevent information loss or fragmentation.
  - **Sub-Agent Parallel Processing**: Multiple specialized sub-agents work in parallel with shared global context fingerprint.
  - **Five-Dimensional Extraction Framework**: Dynamic role inference + Key Facts + Problem Analysis + Core Conclusions + Task & Responsibility Matrix.
  - **Professional Output**: Generates clean, high-quality Markdown meeting minutes and professionally formatted Word documents.
  - **Strict Pure Output**: Final response contains **only** the formal meeting minutes — no greetings, explanations, or extra text.

-----

## 📋 Skill Information

  - **Name**: meeting-lens
  - **Version**: 1.0
  - **Author**: Gao Longbiao (高龙彪)
  - **License**: Apache-2.0
  - **Use Cases**: Long meeting transcripts (10,000+ words), project review meetings, business analysis sessions, strategic workshops, etc.

-----

## 🚀 How to Use

### 1\. Prepare the Input

Save the raw meeting transcript as a `.txt` or `.md` file (UTF-8 encoding recommended).

### 2\. Invoke the Skill

In platforms that support this skill (Claude, Cursor, etc.), use the following prompt:

```markdown
Use the meeting-lens skill to process the following meeting transcript:

[Paste or upload the full meeting transcript here]
```

### 3\. Output

  - Clean Markdown-formatted formal meeting minutes  
  - Automatically generated Word document with professional formatting
  - Output language matches the original transcript (defaults to Chinese)

-----

## 📘 Output Structure

**【Generated Meeting Title】 Meeting Minutes**

**I. Meeting Background and Core Agenda**
**一、会议背景与核心议程**  
(Approximately 300 words, covering motivation, objectives, and key participants)

**II. Key Facts and Information Updates**
(Detailed data, progress, metrics, and examples)

**III. Problem Analysis and Key Challenges**
(Business pain points, cognitive conflicts, and core contradictions)

**IV. Core Conclusions and Management Requirements**
(Decisions made, management red lines, and underlying rationale)

**V. Task Deployment and Responsibility Matrix**

| Responsible Person | Action Items & Delivery Standards | Resource Dependencies | Deadline |
| :--- | :--- | :--- | :--- |
| [Role/Person] | [Clear actions with specific requirements] | [Required support/resources] | [YYYY-MM-DD] |

-----

## 🛠️ Technical Highlights

1.  **Step 1**: Full-context rapid read to extract global context fingerprint
2.  **Step 2**: Adaptive dynamic chunking (4000–5000 characters baseline + 500-char overlap)
3.  **Step 3**: Sub-agents perform parallel five-dimensional deep extraction
4.  **Step 4–5**: Self-verification + global merging and deduplication
5.  **Step 6**: Standardized Markdown rendering
6.  **Step 7**: Export to professionally formatted Word document (SimSun font for Chinese, Small Four size)
7.  **Step 8**: Automatic cleanup of temporary files

-----

## 📄 License

This project is licensed under the Apache License 2.0.

## 👤 Author

**Gao Longbiao**
GitHub: [@gaolongbiao](https://www.google.com/search?q=https://github.com/gaolongbiao)

## ⭐ Support the Project

If Meeting-Lens helps improve your meeting efficiency, please consider giving this repository a ⭐ Star\!
Contributions, issues, and feature requests are welcome\!

## 📬 Contact & Feedback

  - **GitHub Issues**: Feel free to report bugs or suggest improvements
  - **Author on X (Twitter)**: @gaolongbiao

> Making every meeting's value crystal clear.
> **Meeting-Lens — Giving long meetings clear structure and soul.**

```
```
