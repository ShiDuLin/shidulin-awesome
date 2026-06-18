---
name: hello-world
description: 当用户输入 hello-world 时，直接输出 hello world!
---

# Hello World

当用户输入 `hello-world` 时，直接输出 `hello world!`，不做任何额外操作。

## Subagents

当用户输入 `hello-world-subagent` 时，启动一个 subagent 来生成算法代码：读取 `agents/algo-coder.md` 的内容，然后使用 Agent 工具启动 subagent，将读取到的指令作为 prompt 传递，由 subagent 独立完成算法代码生成任务。
