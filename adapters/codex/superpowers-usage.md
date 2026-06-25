# Codex 使用 Superpowers

本仓库计划把 Superpowers 作为完整插件结构放在：

```text
plugins/superpowers/
```

目标是以后可以同时服务：

- Codex App
- Codex CLI
- ChatGPT + Codex 协同开发
- 其他支持 Skills/Plugin 结构的 Agent

## 推荐使用方式

优先使用 Codex 官方插件市场安装 Superpowers：

```text
/plugins
```

搜索：

```text
superpowers
```

然后安装插件。

如果需要使用本仓库中的版本，则应以 `plugins/superpowers/` 为插件根目录，而不是只复制 `skills/` 目录。

## 本仓库路径

```text
plugins/superpowers/.codex-plugin/plugin.json
plugins/superpowers/skills/
```

`plugin.json` 中的关键字段：

```json
"skills": "./skills/"
```

## 与 Codex Hub 规范的关系

用户说“进入 chatgpt 和 codex 协同开发模式”时，应优先遵守 `xsgteamx/codex` 的 Codex Hub 规范：

1. 先读 `README.md`
2. 再读 `AGENTS.md`
3. 再读相关 `playbooks/*`
4. 再读项目 `CONTEXT.md`
5. 然后使用 Superpowers 的流程补强需求澄清、计划、TDD、审查和收尾

Superpowers 不是替代 Codex Hub，而是作为执行方法论增强层。

## 建议任务语句

```text
请按 xsgteamx/codex 的 Codex Hub 规范工作，并使用 Superpowers 的 brainstorming、writing-plans、test-driven-development、requesting-code-review 流程。
本次目标：<目标>
```

## 注意

- 不要因为 Superpowers 要求 TDD，就忽略用户项目实际情况。
- 如果项目没有测试框架，应先建立最小可验证方式，而不是强行大改。
- 如果任务是文档/调研类，不要硬套代码 TDD。
- 如果用户要求快速验证，优先提供最小闭环。
