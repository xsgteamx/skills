# xsgteamx/skills

个人 AI Skills 仓库。

当前收录的是从 [mattpocock/skills](https://github.com/mattpocock/skills) 原样搬运的 Skills，不再做中文改写。

## 当前包含

| Skill | 本仓库路径 | 上游路径 | 说明 |
|---|---|---|---|
| `/grill-me` | `skills/productivity/grill-me/SKILL.md` | `skills/productivity/grill-me/SKILL.md` | 入口 Skill：启动 `/grilling`。 |
| `grilling` | `skills/productivity/grilling/SKILL.md` | `skills/productivity/grilling/SKILL.md` | 核心 Skill：对 plan/design 做持续追问。 |

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
