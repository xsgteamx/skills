---
name: grill-me
description: 在开发项目或方案设计前，启动一次高强度需求拷问，帮助用户把目标、边界、风险、取舍和验收标准问清楚。
disable-model-invocation: true
---

Run a `/grilling` session.

## 使用方式

当用户使用下面这些表达时，进入 `/grill-me`：

- `/grill-me`
- `进入 grill-me 模式`
- `先拷问我这个项目`
- `先不要写代码，先问清楚需求`
- `开发前把所有需要考虑的问题都反问我`

## 行为要求

进入后不要直接写方案、代码或 PRD。

应转入 `grilling` 的工作方式：

1. 一次只问一个最关键的问题。
2. 每个问题都给出 AI 的推荐答案，方便用户确认或修改。
3. 用户回答后继续追问下一个关键分支。
4. 能从代码、README、AGENTS.md、CONTEXT.md、需求文档或已有资料中查到的，不要重复问用户。
5. 信息足够后，再输出结构化结论和可执行任务卡。

## Attribution

Adapted from `mattpocock/skills` under the MIT License. See `../../LICENSES/mattpocock-skills-MIT-LICENSE.md`.
