# Vivek Gupta's Agent Skills

[![skills.sh](https://skills.sh/b/drguptavivek/agent-skills)](https://skills.sh/drguptavivek/agent-skills)

A curated collection of reusable skills for AI coding and research agents. The catalog follows the open Agent Skills format and is installable with the [`vercel-labs/skills`](https://github.com/vercel-labs/skills) CLI.

## Available skills

| Skill | Purpose |
| --- | --- |
| [`zotero-use`](skills/zotero-use/) | Search, retrieve, and review Zotero references; brainstorm from Zotero evidence; and add live Zotero citation fields to Word documents. |
| [`r-ophthal-analysis`](skills/r-ophthal-analysis/) | Run stepwise, researcher-controlled ophthalmology clinical analyses in R/R Markdown, from data audit through publication outputs. |

## Install

List the available skills:

```bash
npx skills add drguptavivek/agent-skills --list
```

Install `zotero-use` interactively:

```bash
npx skills add drguptavivek/agent-skills --skill zotero-use
```

Install `r-ophthal-analysis` interactively:

```bash
npx skills add drguptavivek/agent-skills --skill r-ophthal-analysis
```

Install either skill globally for Codex by adding `--global --agent codex --yes`:

```bash
npx skills add drguptavivek/agent-skills --skill zotero-use --global --agent codex --yes
npx skills add drguptavivek/agent-skills --skill r-ophthal-analysis --global --agent codex --yes
```

The CLI supports Codex, Claude Code, Cursor, Gemini CLI, OpenCode, and many other agents. See the upstream [`vercel-labs/skills` documentation](https://github.com/vercel-labs/skills) for supported agents and installation options.

## Catalog layout

Each skill lives at `skills/<skill-name>/` and contains its own `SKILL.md` entrypoint plus any required references, scripts, or assets.

## Maintenance

Each marketplace entry has a separate canonical repository. Do not edit mirrored skill folders directly:

- [`drguptavivek/zotero-use`](https://github.com/drguptavivek/zotero-use), mirrored by the `Sync zotero-use` workflow.
- [`drguptavivek/r-ophthal-analysis`](https://github.com/drguptavivek/r-ophthal-analysis), mirrored by the `Sync r-ophthal-analysis` workflow.

Both workflows refresh their mirrors daily and can also be run manually.
