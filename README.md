# notes
与 Muse 聊天整理成的文档（AI Agent 平台设计、技术笔记等）

## AI Agent 平台设计

以下文档整理自 2026-10-04 的设计讨论。按主题记录设计方向、适用边界和待确认事项，不代表已有实现。

1. [Agent Runtime SDK 与外层平台的职责边界](agent-platform/01-runtime-boundary.md)
2. [恢复语义与安全恢复点](agent-platform/02-recovery-checkpoints.md)
3. [实时事件、持久化与 SSE 重连](agent-platform/03-streaming-and-persistence.md)
4. [Redis 心跳、执行归属与接管](agent-platform/04-heartbeat-and-takeover.md)
5. [通过执行尝试隔离降低锁风险](agent-platform/05-attempt-isolation.md)——降低锁风险是明确目标；具体数据模型为待确认方案。

阅读顺序建议按上面的编号进行。其中，第四篇定义接管的需求和约束，第五篇讨论满足这些约束的一种实现方式。
