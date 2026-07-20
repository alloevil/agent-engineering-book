# 第 3 章：Agent 核心模式

> 核心论点：Agent 的推理-行动循环有几种经典模式，各有适用场景。

## 3.1 ReAct（Reasoning + Acting）

交替推理和行动：Thought → Action → Observation → Thought → ...

- 优势：可解释、可干预
- 局限：长链路时推理漂移
- 实现：LangChain ReAct Agent、OpenAI function calling loop

## 3.2 Plan-and-Execute

先规划全局计划，再逐步执行。支持重规划。

- 优势：适合复杂多步任务，避免局部最优
- 局限：计划可能过时，需要重规划机制
- 实现：LangGraph Plan-and-Execute

## 3.3 Reflexion

执行后自我反思，从失败中学习。

- 优势：单次任务内自我纠错
- 局限：增加延迟和 token 消耗
- 实现：Reflexion 论文、LATS（Language Agent Tree Search）

## 3.4 Tool-Use Agent

以工具调用为核心驱动。函数调用 vs 工具调用。并行/嵌套工具调用。

## 3.5 Multi-Agent 协作模式

- 主从模式（Orchestrator + Workers）
- 辩论模式（Adversarial Debate）
- 流水线模式（Pipeline Handoff）
- 共享黑板模式（Blackboard）

## 3.6 如何选择模式

任务复杂度 vs 可靠性要求 vs 延迟约束 → 决策矩阵。

---

*本章待展开。*
