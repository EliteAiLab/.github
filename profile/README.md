# Elite AI Lab · 博昇

> **The measure of model merit.** — 模型价值的度量衡

**我们做国产异构算力上的大模型适配与实测。**

不是又一个跑分工具——而是把「模型能不能在这张卡上真正跑好、为什么、提升了多少」变成**可复现、可复核、可对比的证据**。

---

## 我们在解决的问题

国产算力的真问题不在「能不能跑」，而在：

| 问题 | 表现 |
|---|---|
| **适配难** | 算子到底走没走到目标后端？什么时候悄悄退回了 fallback？ |
| **归因难** | 变快了——是因为命中了目标路径，还是因为工况漂移？ |
| **复核难** | 换个人、换台机器，还能得出同一个结论吗？ |

---

## 我们的项目

### EliteMark · 模衡 —— 测量平面

面向 LLM 推理的实测与证据库。为每一次运行生成可复现的**运行指纹**，把「什么硬件 · 什么框架 · 什么算子 · 什么并发 · 什么任务」钉死，让两次测量**可比或不可比**成为一个可判定的问题，而不是靠人记。

> **状态**：本地端 / 汇总端主干可用。公开标准测试集尚未接通跑分引擎——**因此我们不对外发布任何「某模型得多少分」的数字。**

### EliteAdapt —— 适配决策平面

把「遇到什么问题 → 改了什么 → 提升多少 → 在什么工况下成立」变成**结构化对象**，而不是报告文案。每条结论都绑定环境指纹与证据链。

> **状态**：对象模型与证据链协议已成型；与测量平面的对接尚未接线。

---

## 我们坚持的

- **口径先于数字。** 没有 workload 定义的 benchmark 数字，不出。
- **路径先于结论。** 不知道走了哪条后端路径的「性能提升」，不认。
- **不能证伪的，不算证据。**
- **没做出来的，如实标注。** 已知未完成的事写进 README，不写成「已实现」。

---

## 技术栈

Go · vLLM / llama.cpp / Ollama 运行时适配 · 国产算力（昇腾）适配中

---

## 联系

- 邮箱：donaldtang2k@gmail.com

---

<details>
<summary><b>English</b></summary>

**Elite AI Lab** builds reproducible measurement and adaptation tooling for LLM inference on non‑NVIDIA accelerators.

Our thesis: a benchmark number means nothing without the execution path, the environment fingerprint, and a falsifiable claim behind it. We would rather publish nothing than publish a number we cannot reproduce.

Early stage — the skeleton is up, and the gaps are labelled as gaps.

</details>
