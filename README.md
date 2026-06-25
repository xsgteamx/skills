# xsgteamx/skills

个人 AI Skills 仓库。根 README 只做索引和用法说明，具体行为规则写在各自的 `SKILL.md` 里。

## 🧩 当前包含的 Skills

| Skill | 路径 | 简介 |
|---|---|---|
| 🔥 `/grill-me` | `productivity/grill-me/SKILL.md` | 入口 Skill：启动开发前需求拷问流程。 |
| 🧠 `grilling` | `productivity/grilling/SKILL.md` | 核心 Skill：持续追问项目目标、边界、风险、取舍与验收标准。 |

## 📁 仓库结构

仓库本身已经叫 `skills`，所以不再额外套一层 `skills/` 目录。

```text
productivity/
  grill-me/
    SKILL.md
  grilling/
    SKILL.md
LICENSES/
  mattpocock-skills-MIT-LICENSE.md
THIRD_PARTY_NOTICES.md
```

后续新增类别时，直接在根目录下增加分类：

```text
engineering/
research/
writing/
devops/
bio/
```

## 💬 在 ChatGPT 里怎么使用

ChatGPT 不会自动长期挂载这个 GitHub 仓库里的 Skills。要使用时，直接在对话里点名仓库和 Skill。

### 轻量用法

适合你已经知道要用哪个 Skill，不要求我重新读取仓库最新内容：

```text
使用我的 xsgteamx/skills 里的 /grill-me 模式，拷问这个项目：<项目目标>
```

或者更短：

```text
进入 grill-me 模式，先不要写方案，先拷问我这个项目：<项目目标>
```

### 严格用法

适合你刚更新过仓库，希望我按 GitHub 里的最新 `SKILL.md` 执行：

```text
请读取 GitHub 仓库 xsgteamx/skills 的 README.md、productivity/grill-me/SKILL.md 和 productivity/grilling/SKILL.md，然后按 /grill-me 开始拷问我这个项目：<项目目标>
```

### 和 Codex 协同开发时

```text
进入chatgpt和codex协同开发模式。先使用 xsgteamx/skills 的 /grill-me，把需求问清楚；信息足够后，再输出可交给 Codex 执行的任务卡。

本次目标：<目标>
```

## 📌 维护约定

- 根 README 只维护 Skill 清单、目录结构和入口用法。
- 每个 Skill 的触发方式、行为规则、输出格式，放在对应目录的 `SKILL.md`。
- 后续新增 Skill 时，只需要在上面的表格里补一行。
- 复杂流程建议拆成：入口 Skill + 核心 Skill。

## 🙏 Attribution

`grill-me` / `grilling` 改编自 `mattpocock/skills`，原项目使用 MIT License。

第三方说明见：

```text
THIRD_PARTY_NOTICES.md
LICENSES/mattpocock-skills-MIT-LICENSE.md
```
