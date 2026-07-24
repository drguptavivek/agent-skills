# Vivek Gupta's Agent Skills

[![skills.sh](https://skills.sh/b/drguptavivek/agent-skills)](https://skills.sh/drguptavivek/agent-skills)

A curated collection of reusable skills for AI coding and research agents. The catalog follows the open Agent Skills format and is installable with the [`vercel-labs/skills`](https://github.com/vercel-labs/skills) CLI.

## Available skills

| Skill | Purpose |
| --- | --- |
| [`zotero-use`](skills/zotero-use/) | Search, retrieve, and review Zotero references; brainstorm from Zotero evidence; and add live Zotero citation fields to Word documents. |

## Install

List the available skills:

```bash
npx skills add drguptavivek/agent-skills --list
```

Install `zotero-use` interactively:

```bash
npx skills add drguptavivek/agent-skills --skill zotero-use
```

Install it globally for Codex:

```bash
npx skills add drguptavivek/agent-skills --skill zotero-use --global --agent codex --yes
```

The CLI supports Codex, Claude Code, Cursor, Gemini CLI, OpenCode, and many other agents. See the upstream [`vercel-labs/skills` documentation](https://github.com/vercel-labs/skills) for supported agents and installation options.

## Catalog layout

Each skill lives at `skills/<skill-name>/` and contains its own `SKILL.md` entrypoint plus any required references, scripts, or assets.

## Maintenance

The canonical source for `zotero-use` is [`drguptavivek/zotero-use`](https://github.com/drguptavivek/zotero-use). Do not edit its marketplace mirror directly. The `Sync zotero-use` GitHub Actions workflow refreshes the mirror daily and can also be run manually.
