# 第 4 章：主流 Agent 框架

> 核心论点：框架是 Harness 的实现载体。2026 年的框架分为两类——通用编排框架和垂直集成 Agent。

## 4.1 通用编排框架：LangGraph

图状态机，节点=步骤，边=转移。State、Node、Edge、Conditional Edge。

## 4.2 终端 Coding Agent

### Pi
极简主义，"提供原语，不提供功能"。仅 read、write、edit、bash。

### oh-my-pi（omp）
出厂即顶配：Hash-anchored edits、LSP、DAP、Hindsight memory、Sub-agents、Time-traveling rules。

### Claude Code
Anthropic 官方，ReAct + Tool Use，沙箱 + 审批。

### Codex CLI
OpenAI 官方，沙箱 + approval 模式。

## 4.3 长期运行 Agent：OpenClaw

7×24 持续运行。记忆持久化 + 定时任务 + 多通道消息 + 多代理协调。

## 4.4 框架选型决策矩阵

按类型、Harness 深度、适合场景对比。

---

*本章待展开。*
