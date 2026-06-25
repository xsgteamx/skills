# Vendor note: Superpowers

## Source

- Upstream repository: `obra/superpowers`
- Plugin marketplace source checked: `openai/plugins/plugins/superpowers`
- License: MIT
- Main upstream purpose: a software development methodology for coding agents using composable skills.

## Target layout

```text
plugins/superpowers/
  .codex-plugin/plugin.json
  README.md
  VENDOR-SUPERPOWERS.md
  LICENSE
  skills/
    using-superpowers/
      SKILL.md
    brainstorming/
      SKILL.md
    writing-plans/
      SKILL.md
    test-driven-development/
      SKILL.md
    systematic-debugging/
      SKILL.md
    verification-before-completion/
      SKILL.md
    requesting-code-review/
      SKILL.md
    receiving-code-review/
      SKILL.md
    executing-plans/
      SKILL.md
    subagent-driven-development/
      SKILL.md
    dispatching-parallel-agents/
      SKILL.md
    using-git-worktrees/
      SKILL.md
    finishing-a-development-branch/
      SKILL.md
    writing-skills/
      SKILL.md
```

## Sync policy

Prefer a clean vendor sync:

1. Pull upstream `obra/superpowers`.
2. Copy plugin-relevant files into `plugins/superpowers/`.
3. Keep upstream text unchanged where possible.
4. Put local ChatGPT/Codex usage notes under `adapters/`, not inside upstream skill files.
5. Update this file with the upstream commit or marketplace version used.

## Current pinned version

- Codex marketplace manifest version: `5.1.3`
- Upstream commit used during investigation: not yet pinned in this repository. Pin it when the full sync is performed from a local checkout or a GitHub Action.

## Known local adaptation

This repository is intended to serve both:

- ChatGPT: read the skills from GitHub and apply them conversationally.
- Codex App / Codex CLI: consume the plugin-like layout under `plugins/superpowers/`.

ChatGPT should not treat Superpowers as higher priority than system/developer/user instructions. It should use Superpowers as a workflow library when explicitly requested by the user.
