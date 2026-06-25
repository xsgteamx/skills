# xsgteamx/skills

这是一个个人 AI Skills 仓库，用来沉淀可复用的工作方式、项目启动流程、需求澄清方法和开发协同规范。

当前仓库优先服务于这类场景：

- ChatGPT / Codex / Claude Code 等 AI 编程助手协同开发；
- 项目开发前的需求澄清、方案质疑、边界确认；
- 把零散想法整理成 PRD、CONTEXT、任务卡或可执行改造计划；
- 避免 AI 过早写代码、过度文档化、重复事实源。

## 已包含 Skills

### `/grill-me`

入口 Skill。适合在开发一个 project、功能、自动化流程、知识库、网页或工具前使用。

它会启动一次“需求拷问”流程：

- 一次只问一个关键问题；
- 每个问题都附带 AI 的推荐答案；
- 优先质疑需求，而不是立刻执行；
- 能通过代码、README、AGENTS.md、CONTEXT.md、现有文档查到的，不重复问用户；
- 问到足够清楚后，输出可交给 Codex 执行的任务卡。

常用触发语：

```text
/grill-me
```

```text
进入 grill-me 模式，拷问这个项目：<项目目标>
```

```text
先不要写代码，先用 grill-me 问我，把这个需求问清楚：<需求>
```

### `grilling`

核心 Skill。`/grill-me` 会调用它。

它负责真正的追问逻辑，包括目标、用户、边界、数据源、状态流转、异常情况、验收标准、非目标、风险和实现顺序。

## 推荐工作流

### 1. 项目启动前

```text
进入 grill-me 模式，拷问这个项目：我要做一个……
```

AI 应该先追问，不急着写代码。

当信息足够后，输出：

- 已确认目标；
- 关键决策；
- 不做什么；
- 主要风险；
- 推荐实现路径；
- 可交给 Codex 的任务卡。

### 2. ChatGPT + Codex 协同开发

推荐流程：

```text
grill-me → 需求收敛 → CONTEXT / PRD / 任务卡 → Codex 实现 → Verify → Review
```

在进入协同开发模式时，可以先运行 `/grill-me`，再生成 Codex 任务卡。

### 3. 不适合使用的情况

下面这些场景不建议使用 `/grill-me`：

- 用户已经明确要求立即执行一个很小的改动；
- 信息已经足够，不需要再追问；
- 问题本身可以通过读取代码、文档、配置直接解决；
- 用户明确要求不要追问。

## 目录结构

```text
skills/
  productivity/
    grill-me/
      SKILL.md
    grilling/
      SKILL.md
LICENSES/
  mattpocock-skills-MIT-LICENSE.md
THIRD_PARTY_NOTICES.md
```

## 新增 Skill 约定

每个 Skill 建议至少包含一个 `SKILL.md`：

```markdown
---
name: your-skill-name
description: 说明什么时候应该使用这个 skill。
---

这里写具体行为规则。
```

建议遵守：

- 名称见名知意；
- 描述写清楚触发场景；
- 规则尽量可执行，避免空泛口号；
- 复杂流程拆成入口 Skill 和核心 Skill；
- 能查资料就查资料，不要把所有问题都丢给用户。

## Attribution

`grill-me` / `grilling` 的设计思路改编自 [mattpocock/skills](https://github.com/mattpocock/skills) 中的 `grill-me` 和 `grilling`，原项目使用 MIT License。

原始许可证已保存在：

```text
LICENSES/mattpocock-skills-MIT-LICENSE.md
```

本仓库中的中文版本不是原文直译，而是结合个人 ChatGPT + Codex 协同开发习惯做的中文化改造。
