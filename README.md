# xsgteamx/skills

个人 AI Skills 仓库，用来收集可复用的 AI 工作流与 Agent 行为规范。

当前收录的是从 [mattpocock/skills](https://github.com/mattpocock/skills) 原样搬运的 Skills。

原则：

- `SKILL.md` 尽量保持上游原文，不做中文改写；
- 中文说明、使用方式、命名解释放在根 `README.md`；
- 如果以后要做中文增强版，建议另建新 Skill，例如 `skills/productivity/grill-me-cn/`，不要覆盖上游原版。

## 当前包含

| Skill | 中文别名 | 本仓库路径 | 上游路径 | 说明 |
|---|---|---|---|---|
| `/grill-me` | 拷问我 | `skills/productivity/grill-me/SKILL.md` | `skills/productivity/grill-me/SKILL.md` | 入口 Skill：启动 `/grilling`。 |
| `grilling` | 持续盘问 | `skills/productivity/grilling/SKILL.md` | `skills/productivity/grilling/SKILL.md` | 核心 Skill：围绕 plan/design 持续追问，直到达成共同理解。 |

## 中文名怎么理解

`grill-me` 建议翻译成：**拷问我**。

原因：

- `grill` 在这里不是“烧烤”，而是口语里的“连续追问、盘问、压力测试”；
- `/grill-me` 的语气比普通的“问我问题”更强，强调在开发前把方案、边界、风险和取舍问透；
- “盘问我”更温和，但力度不如“拷问我”；
- “审问我”太像法律/刑侦语境，不适合项目开发；
- “灵魂拷问我”太口语化，可以聊天时说，但不适合作为正式别名。

所以 README 里使用：

```text
/grill-me（拷问我）
grilling（持续盘问）
```

注意：中文名只是帮助理解，不替代 Skill 的真实名称。真实触发名仍然是 `/grill-me` 和 `grilling`。

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

这里保留上游的 `skills/...` 目录结构。  
所以 GitHub 页面上看起来会是 `xsgteamx/skills/skills/...`，这是因为仓库名叫 `skills`，同时上游目录也叫 `skills`。

## 在 ChatGPT 里使用

轻量用法：

```text
使用我的 xsgteamx/skills 里的 /grill-me，拷问这个项目：<项目目标>
```

严格用法：

```text
请读取 GitHub 仓库 xsgteamx/skills 的 README.md、skills/productivity/grill-me/SKILL.md 和 skills/productivity/grilling/SKILL.md，然后按 /grill-me 开始拷问我这个项目：<项目目标>
```

和 Codex 协同开发时：

```text
进入chatgpt和codex协同开发模式。先使用 xsgteamx/skills 的 /grill-me，把需求问清楚；信息足够后，再输出可交给 Codex 执行的任务卡。

本次目标：<目标>
```

## Attribution

`grill-me` / `grilling` 原样复制自 `mattpocock/skills`，原项目使用 MIT License。

第三方说明见：

```text
THIRD_PARTY_NOTICES.md
LICENSES/mattpocock-skills-MIT-LICENSE.md
```
