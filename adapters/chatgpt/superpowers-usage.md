# ChatGPT 使用 Superpowers

当用户说：

```text
使用 Superpowers
使用 xsgteamx/skills 里的 Superpowers
进入 chatgpt 和 codex 协同开发模式，并使用 Superpowers
```

ChatGPT 应按以下方式使用本仓库内容。

## 读取顺序

1. `README.md`
2. `plugins/superpowers/README.md`
3. `plugins/superpowers/VENDOR-SUPERPOWERS.md`
4. `plugins/superpowers/skills/using-superpowers/SKILL.md`
5. 与当前任务匹配的具体 skill，例如：
   - 新功能/新项目：`brainstorming`
   - 写任务卡：`writing-plans`
   - 修 Bug：`systematic-debugging`
   - 验证修复：`verification-before-completion`
   - 代码审查：`requesting-code-review`
   - 收尾：`finishing-a-development-branch`

## 本地优先级

Superpowers 是工作流库，不得覆盖更高优先级指令。

优先级：

1. ChatGPT 系统/开发者指令
2. 用户当前明确要求
3. Project / 仓库内已有规范，例如 `AGENTS.md`、`CONTEXT.md`
4. Superpowers skills
5. 通用经验

## 和用户习惯的适配

用户偏好“先质疑、少闭门造车、避免过度文档化”。因此使用 Superpowers 时：

- 可以使用 brainstorming，但不要机械地无限追问。
- 对小任务可以给短设计，不强行写长篇 spec。
- 需要进入 Codex 执行时，输出可复制的任务卡。
- 对已有代码仓库，先读 README/AGENTS/CONTEXT，再设计。
- 发现风险要直接指出，不要只顺着用户需求写。

## 推荐触发语

```text
使用 Superpowers，帮我把这个需求先拷问清楚，再输出给 Codex 的任务卡：<目标>
```

```text
进入 chatgpt 和 codex 协同开发模式，使用 Superpowers 流程推进。
本次目标：<目标>
```

## 输出习惯

ChatGPT 不需要逐字声明“我正在调用某某 Skill”。更适合输出：

1. 先确认目标和风险；
2. 必要时一次只问一个关键问题；
3. 信息足够后给 2-3 个方案和推荐；
4. 最后输出 Codex 可执行任务卡。
