---
layout: section
---

# 🎸 Module 7

## Vibe Coding

<div class="text-sm opacity-60 mt-4">"不写代码"的编程革命</div>

---
layout: quote
---

# "I just see things, say things, run things, and copy-paste things, and it mostly works."

<div class="mt-4 text-right opacity-70">
  — Andrej Karpathy, 2025
</div>

<div class="mt-6 text-sm">
  前特斯拉 AI 总监、OpenAI 联合创始人提出的全新编程范式
</div>

---
layout: default
---

# 什么是 Vibe Coding？

<v-clicks>

- 🎸 **核心理念："跟着感觉走"**
  - 用自然语言描述你想要什么
  - AI 负责生成代码
  - 你负责审查和迭代

- 🔄 **工作流**
  - 描述需求 → AI 生成 → 运行测试 → 迭代优化

- 🎯 **关键转变**
  - ~~手写每一行代码~~ → 描述意图
  - ~~调试语法错误~~ → 审查逻辑
  - ~~查阅 API 文档~~ → 对话式开发

- ⚠️ **注意：Vibe Coding ≠ 不需要编程知识**
  - 你仍需理解代码来做出正确判断

</v-clicks>

---
layout: default
---

# Vibe Coding 工具链

<div class="grid grid-cols-2 gap-6 mt-6">

<div v-click class="p-4 rounded-lg" style="background: linear-gradient(135deg, #1a365d, #2c5282);">
  <div class="flex items-center gap-2 mb-2">
    <carbon-code class="text-xl text-blue-300" />
    <span class="font-bold">Cursor</span>
  </div>
  <div class="text-sm opacity-70">VS Code 分支，AI-First 编辑器</div>
  <div class="text-xs mt-2 opacity-50">Tab 补全 · Chat · Composer 多文件编辑</div>
</div>

<div v-click class="p-4 rounded-lg" style="background: linear-gradient(135deg, #2d3748, #553c9a);">
  <div class="flex items-center gap-2 mb-2">
    <carbon-terminal class="text-xl text-purple-300" />
    <span class="font-bold">Claude Code</span>
  </div>
  <div class="text-sm opacity-70">Anthropic 官方终端 Agent</div>
  <div class="text-xs mt-2 opacity-50">命令行原生 · 自主执行 · 深度推理</div>
</div>

<div v-click class="p-4 rounded-lg" style="background: linear-gradient(135deg, #553c9a, #9b2c2c);">
  <div class="flex items-center gap-2 mb-2">
    <carbon-rocket class="text-xl text-pink-300" />
    <span class="font-bold">Windsurf</span>
  </div>
  <div class="text-sm opacity-70">Codeium 出品的 AI 编辑器</div>
  <div class="text-xs mt-2 opacity-50">Cascade 工作流 · 上下文感知 · 自动操作</div>
</div>

<div v-click class="p-4 rounded-lg" style="background: linear-gradient(135deg, #1a365d, #38a169);">
  <div class="flex items-center gap-2 mb-2">
    <carbon-model-alt class="text-xl text-green-300" />
    <span class="font-bold">Antigravity (Google)</span>
  </div>
  <div class="text-sm opacity-70">Google DeepMind 的编码助手</div>
  <div class="text-xs mt-2 opacity-50">Gemini 原生 · 浏览器控制 · 技能系统</div>
</div>

</div>

---
layout: default
---

# Vibe Coding 实战流程

```mermaid
graph LR
    A["💡 想法"] --> B["📝 描述需求"]
    B --> C["🤖 AI 生成代码"]
    C --> D["▶️ 运行测试"]
    D --> E{"✅ 满意？"}
    E -->|"不满意"| F["🔄 反馈迭代"]
    F --> C
    E -->|"满意"| G["🚀 部署上线"]

    style A fill:#667eea,color:#fff
    style C fill:#764ba2,color:#fff
    style G fill:#38a169,color:#fff
```

<v-click>

<div class="grid grid-cols-3 gap-4 mt-6">

<div class="p-3 rounded-lg text-center text-sm" style="background: rgba(102,126,234,0.15);">
  <div class="font-bold">Step 1</div>
  <div class="opacity-70 mt-1">"创建一个 Todo App<br/>使用 Vue 3 + Pinia"</div>
</div>

<div class="p-3 rounded-lg text-center text-sm" style="background: rgba(118,75,162,0.15);">
  <div class="font-bold">Step 2</div>
  <div class="opacity-70 mt-1">AI 生成完整项目<br/>组件、路由、状态管理</div>
</div>

<div class="p-3 rounded-lg text-center text-sm" style="background: rgba(56,161,105,0.15);">
  <div class="font-bold">Step 3</div>
  <div class="opacity-70 mt-1">"加上暗色模式<br/>和动画过渡效果"</div>
</div>

</div>

</v-click>

---
layout: center
---

# 🗺️ AI 学习路线图

```mermaid
graph TD
    A["🧩 AI 基础概念"] --> B["🛠️ Prompt Engineering"]
    B --> C["🔌 MCP 工具连接"]
    C --> D["🤖 Agent 构建"]
    D --> E["🎸 Vibe Coding"]

    F["🎨 生图模型"] --> E
    G["💻 编码模型"] --> E

    A --> F
    A --> G

    style A fill:#667eea,color:#fff
    style E fill:#f093fb,color:#000
    style F fill:#e53e3e,color:#fff
    style G fill:#38a169,color:#fff
```

<div class="mt-4 text-lg">
  从理解 AI → 使用 AI → 构建 AI 应用 → <strong>用 AI 写代码</strong>
</div>

---
layout: center
class: text-center
---

# 感谢学习！🎉

<div class="text-2xl mt-4" style="background: linear-gradient(135deg, #667eea, #764ba2); -webkit-background-clip: text; -webkit-text-fill-color: transparent;">
  AI 新纪元 — 从入门到 Vibe Coding
</div>

<div class="mt-8 text-sm opacity-50">
  <carbon-logo-github class="inline" /> 课程源码开放 · 持续更新
</div>

<div class="mt-4">
  <span class="px-4 py-2 rounded-full text-sm" style="background: linear-gradient(135deg, #667eea, #764ba2); color: white;">
    开始你的 AI 之旅 →
  </span>
</div>
