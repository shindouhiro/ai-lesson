---
layout: section
---

# 🧩 Module 1

## AI 与大模型基础

<div class="text-sm opacity-60 mt-4">理解 AI 的核心概念与演进历程</div>

---
layout: default
---

# AI 发展简史

<div class="timeline">

```mermaid
timeline
    title AI 技术演进
    1950s-1980s : 规则系统 (Expert Systems)
                : 基于人工编写的规则
    1990s-2010s : 机器学习 (ML)
                : 从数据中学习模式
    2012-2017   : 深度学习 (DL)
                : 神经网络的复兴
    2017-2022   : Transformer 时代
                : Attention Is All You Need
    2022-Now    : 大模型 (LLM) 时代
                : GPT / Claude / Gemini
```

</div>

<v-click>

> 💡 我们正处于 AI 技术的**寒武纪大爆发**时期

</v-click>

<!--
AI 并非一夜之间出现的技术，它经历了 70 多年的发展。
Transformer 架构在 2017 年彻底改变了 AI 的格局。
-->

---
layout: two-cols
---

# 什么是大语言模型？

<v-clicks>

- 🧠 **Large Language Model (LLM)**
  - 在海量文本上训练的深度神经网络
- 📝 **核心能力：预测下一个 Token**
  - "今天天气" → "真好" (概率最高)
- 🔤 **Token 化**
  - 文字被分割为最小处理单元
  - "人工智能" → ["人工", "智能"]
- 🎯 **涌现能力 (Emergence)**
  - 当模型足够大时，出现意想不到的能力

</v-clicks>

::right::

<div class="ml-4 mt-4">

```mermaid
graph TD
    A["📥 输入文本"] --> B["🔤 Token 化 + Embedding"]
    B --> C["🧠 Transformer 层 x N"]
    C --> D["📤 预测下一个 Token"]
    D -->|"循环"| A

    style A fill:#667eea,color:#fff,stroke:#667eea
    style C fill:#764ba2,color:#fff,stroke:#764ba2
    style D fill:#f093fb,color:#000,stroke:#f093fb
```

</div>

---
layout: default
---

# 模型参数与能力

参数量决定了模型的"大脑容量"

<div class="grid grid-cols-4 gap-4 mt-8">

<div v-click class="p-4 rounded-lg text-center" style="background: linear-gradient(135deg, #2d3748, #4a5568);">
  <div class="text-3xl font-bold text-blue-300">7B</div>
  <div class="text-sm mt-2 opacity-70">轻量级</div>
  <div class="text-xs mt-1 opacity-50">Llama 3.1 7B</div>
  <div class="mt-2 text-xs">✅ 简单对话<br/>⚠️ 推理能力有限</div>
</div>

<div v-click class="p-4 rounded-lg text-center" style="background: linear-gradient(135deg, #2d3748, #553c9a);">
  <div class="text-3xl font-bold text-purple-300">70B</div>
  <div class="text-sm mt-2 opacity-70">专业级</div>
  <div class="text-xs mt-1 opacity-50">Llama 3.1 70B</div>
  <div class="mt-2 text-xs">✅ 复杂推理<br/>✅ 代码生成</div>
</div>

<div v-click class="p-4 rounded-lg text-center" style="background: linear-gradient(135deg, #2d3748, #9b2c2c);">
  <div class="text-3xl font-bold text-red-300">405B</div>
  <div class="text-sm mt-2 opacity-70">旗舰级</div>
  <div class="text-xs mt-1 opacity-50">Llama 3.1 405B</div>
  <div class="mt-2 text-xs">✅ 接近 GPT-4 级<br/>✅ 多语言精通</div>
</div>

<div v-click class="p-4 rounded-lg text-center" style="background: linear-gradient(135deg, #2d3748, #d69e2e);">
  <div class="text-3xl font-bold text-yellow-300">1T+</div>
  <div class="text-sm mt-2 opacity-70">超级模型</div>
  <div class="text-xs mt-1 opacity-50">GPT-4 / Claude Opus</div>
  <div class="mt-2 text-xs">✅ 顶级推理<br/>✅ 多模态</div>
</div>

</div>

<v-click>

<div class="mt-6 text-center text-sm opacity-60">
  ⚡ 参数量 ≠ 一切 — 架构设计、训练数据质量和训练方法同样关键
</div>

</v-click>

---
layout: default
---

# 模型家族一览 (1/2)

<div class="grid grid-cols-2 gap-6 mt-6">

<div v-click class="p-4 rounded-lg border border-gray-600">
  <div class="flex items-center gap-2 mb-2">
    <simple-icons-openai class="text-xl text-green-400" />
    <span class="font-bold">OpenAI — GPT 系列</span>
  </div>
  <div class="text-sm opacity-70">GPT-4o · o1 · o3 · GPT Image 2</div>
  <div class="text-xs mt-1 opacity-50">多模态先驱，推理能力领先</div>
</div>

<div v-click class="p-4 rounded-lg border border-gray-600">
  <div class="flex items-center gap-2 mb-2">
    <mdi-robot class="text-xl text-orange-400" />
    <span class="font-bold">Anthropic — Claude 系列</span>
  </div>
  <div class="text-sm opacity-70">Haiku · Sonnet · Opus</div>
  <div class="text-xs mt-1 opacity-50">编码与长文本之王</div>
</div>

<div v-click class="p-4 rounded-lg border border-gray-600">
  <div class="flex items-center gap-2 mb-2">
    <simple-icons-google class="text-xl text-blue-400" />
    <span class="font-bold">Google — Gemini 系列</span>
  </div>
  <div class="text-sm opacity-70">Flash · Pro · Ultra</div>
  <div class="text-xs mt-1 opacity-50">原生多模态，百万上下文</div>
</div>

<div v-click class="p-4 rounded-lg border border-gray-600">
  <div class="flex items-center gap-2 mb-2">
    <simple-icons-meta class="text-xl text-blue-500" />
    <span class="font-bold">Meta — LLaMA 系列</span>
  </div>
  <div class="text-sm opacity-70">LLaMA 3.1 · 3.2 · 4</div>
  <div class="text-xs mt-1 opacity-50">开源之王，推动民主化</div>
</div>

</div>

---
layout: default
---

# 模型家族一览 (2/2)

<div class="grid grid-cols-2 gap-6 mt-6">

<div v-click class="p-4 rounded-lg border border-gray-600">
  <div class="flex items-center gap-2 mb-2">
    <carbon-model-alt class="text-xl text-cyan-400" />
    <span class="font-bold">DeepSeek</span>
  </div>
  <div class="text-sm opacity-70">DeepSeek-V3 · R1</div>
  <div class="text-xs mt-1 opacity-50">中国开源强者，MoE 架构</div>
</div>

<div v-click class="p-4 rounded-lg border border-gray-600">
  <div class="flex items-center gap-2 mb-2">
    <carbon-cloud class="text-xl text-indigo-400" />
    <span class="font-bold">xAI — Grok 系列</span>
  </div>
  <div class="text-sm opacity-70">Grok 3 · Grok 3.5</div>
  <div class="text-xs mt-1 opacity-50">Elon Musk 旗下，实时搜索</div>
</div>

</div>
