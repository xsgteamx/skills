# Superpowers

This directory vendors the upstream Superpowers plugin structure so the repository can be reused by multiple coding-agent harnesses, especially Codex App / Codex CLI.

Upstream:

- Repository: https://github.com/obra/superpowers
- Author: Jesse Vincent / Prime Radiant
- License: MIT
- Vendored source: `openai/plugins/plugins/superpowers` manifest plus `obra/superpowers` skills and supporting files

## Why keep this under `plugins/superpowers/`?

Codex plugins are not just loose `SKILL.md` files. A plugin keeps its manifest at:

```text
plugins/<name>/.codex-plugin/plugin.json
```

and points to its skill directory with:

```json
"skills": "./skills/"
```

Keeping the upstream layout makes this repository usable later for Codex, while still allowing ChatGPT to read the same skills manually when requested.

## Local policy

- Keep upstream files as close to original as possible.
- Put Chinese usage notes and local workflow preferences outside this directory, under `adapters/` or the root `README.md`.
- Do not rewrite upstream `SKILL.md` files unless intentionally forking.
- When updating from upstream, refresh this directory and update `VENDOR-SUPERPOWERS.md`.

## Current status

This directory is being introduced as a vendor target. The manifest and core documentation are present first; skill files should be synced from upstream into `plugins/superpowers/skills/`.
