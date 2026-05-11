# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this repo is

An **awesome list**: a single curated catalog (`README.md`) of tools, libraries, MCP servers, and frameworks that power AI coding agents. There is no source code, no build step, and no application to run. The "deliverable" is the README itself plus the CI that validates it.

Repo contents:

- `README.md` — the catalog (the only file most edits touch)
- `LICENSE`, `.lycheeignore`, `.markdownlint.json` — config
- `.github/` — PR template, issue templates (`add-tool.yml`, `remove-tool.yml`), and two workflows (`lint.yml`, `links.yml`)

## Validation commands

The two CI jobs run on every push/PR and must pass. Reproduce locally before committing:

```bash
# Markdown lint (matches .github/workflows/lint.yml)
npx -y markdownlint-cli2 "README.md"

# Link check (matches .github/workflows/links.yml)
lychee --no-progress --max-concurrency 8 --accept 200,206,429 ./README.md
```

`.markdownlint.json` disables MD013 (line length), MD033 (raw HTML — used in the hero badges), MD036 (emphasis-as-heading), MD041 (first-line-heading), and sets MD024 to `siblings_only`. `.lycheeignore` skips x.com, twitter.com, linkedin.com, openai.com, reddit.com (all routinely bot-block) and `file://` URLs.

## Entry format (load-bearing — CI does not check this; reviewers do)

```markdown
- [Tool Name](https://github.com/owner/repo) - One-sentence description ending with a period.
  - **Strengths:** short phrase; another phrase; up to three phrases.
  - **Caveats:** short phrase; up to two phrases.
```

Rules (from `.github/PULL_REQUEST_TEMPLATE.md` and `.github/ISSUE_TEMPLATE/add-tool.yml`):

- Description is **one sentence, ≤120 characters, ends with a period**.
- **Strengths** and **Caveats** are nested bullets with 2-space indentation, semicolon-separated phrases, period-terminated. Use `**Caveats:** None notable.` if truly none.
- Entries are **alphabetical within their subsection** (case-insensitive; `gstack` sits between `graphify` and `Karpathy-...`).
- Mark proprietary or source-available licensing inline; default assumption is open source.
- **One tool per PR** — do not bundle additions unless explicitly told to.
- Tool must be **actively maintained** and **focused on AI coding agents or supporting infrastructure** (the agents themselves like Claude Code/Cursor live in their own repos and are intentionally excluded; this list is the ecosystem around them).

## Inclusion philosophy

`README.md:37` is load-bearing: *"Inclusion is based on visible community use rather than star counts."*

- **Do not add per-entry star counts** (numeric or badge). This was a deliberate design choice.
- The **Featured Tools** hero section at the top (`README.md:18–32`) is the *only* place stars are shown — via dynamic `img.shields.io/github/stars` badges for ~8 hand-picked tools. Don't expand this section casually.
- When adding/removing entries, update the **Tools count badge** (`README.md:12`, currently `tools-131-blue.svg`). The Categories badge (line 13) tracks subsection count, not section count.

## Section taxonomy

There are 5 top-level sections and 27 subsections. The authoritative list lives in the `section` dropdown of `.github/ISSUE_TEMPLATE/add-tool.yml` — consult it before placing a new entry. Top-level groupings:

1. **Extensions, Skills & Rules** — skills, plugins, rules, MCP servers, curated lists, methodologies, marketplaces
2. **Agent SDKs & Frameworks** — vendor SDKs, orchestration, lightweight/typed, structured output, stateful
3. **Supporting Infrastructure** — memory, vector DBs, codebase context, sandboxing, workflow orchestration, evaluation, observability, prompt management, benchmarks, test generation, local LLM runners
4. **Learning Resources** — articles, tutorials, books, podcasts, datasets
5. **Community** — flat list of forums/feeds

Section choice matters: a multi-agent orchestration platform goes under *Orchestration Frameworks*, not *Claude Code Skills & Plugins*, even if it ships Claude-flavored skills.

## When researching candidate tools

Before adding an entry, verify stats with `gh api repos/OWNER/REPO --jq '{stars: .stargazers_count, pushed: .pushed_at, license: .license.spdx_id, archived: .archived, description: .description}'`. Treat star counts and dates reported by web-search agents as unverified — confirm via `gh api` before writing them into a PR description or commit message.

## What not to do

- Don't create new top-level sections or subsections without explicit user direction — the taxonomy is stable.
- Don't reorder existing entries beyond fixing alphabetical drift you encounter.
- Don't reflow descriptions to use bullets, em-dashes, or multi-sentence prose — the one-sentence-with-period rule is enforced visually for scannability.
- Don't add CONTRIBUTING.md, ROADMAP.md, or other meta docs unless asked; the issue/PR templates already encode the rules.
