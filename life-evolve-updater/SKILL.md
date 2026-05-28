---
name: life-evolve-updater
description: Update a personal life-evolve repository from evidence. Use when the user asks to maintain final.md, frontier.md, donelist.md, memory.md, soul.md, hobbies.md, personal strategy, life history, project completion records, or hobby-to-business surfaces. The skill scans available evidence, separates facts from inferences, updates the six living documents coherently, and preserves privacy boundaries.
---

# Life Evolve Updater

Maintain a living personal strategy repository without turning it into vague journaling.

The canonical files are:

- `final.md`: long-horizon strategy and current final thesis.
- `frontier.md`: frontier map, external opportunities, and capability frontier.
- `donelist.md`: evidence-backed completed work and shipped artifacts.
- `memory.md`: life timeline, durable facts, biographical reconstruction.
- `soul.md`: temperament, decision rules, values, operating principles.
- `hobbies.md`: serious interests that can become side businesses.

## Operating Principles

1. Evidence first. Use local files, Git history, deployed products, public links, logs, notes, and user statements.
2. Mark inference. If a claim is inferred rather than directly evidenced, label it.
3. Preserve privacy. Do not place raw chats, secrets, credentials, private database dumps, or sensitive third-party data into public repos.
4. Update as a system. A new product launch may affect `donelist.md`, `final.md`, `hobbies.md`, and `soul.md` together.
5. Keep the user's actual shape. Do not normalize them into generic productivity advice.

## Quick Workflow

1. Identify the target repository and whether it is private or public.
2. Read existing six files if present.
3. Gather evidence:
   - local Git repos and recent commits;
   - README/package metadata;
   - local memory files and notes;
   - user-provided product status;
   - public pages only when current external status matters.
4. Build an evidence inventory with source paths and dates.
5. Update each file:
   - `final.md`: revise the strategic thesis only if evidence changes priorities.
   - `frontier.md`: revise frontier opportunities and constraints.
   - `donelist.md`: add shipped/built work with repo/path/source evidence.
   - `memory.md`: add life facts, chronology, and durable context.
   - `soul.md`: update operating rules and decision constraints.
   - `hobbies.md`: evaluate hobby-to-business optionality.
6. Run a completion audit:
   - every explicit user request has a file;
   - each factual claim has evidence or is marked as inference;
   - private material is not leaked into public artifacts;
   - repo status is clean or changes are intentionally staged.

## Evidence Scanning

Prefer structured scans over manual impressions.

For local Git repositories:

```bash
find ~/GitHub -maxdepth 2 -type d -name .git
```

For each repo, collect:

- repo name and path;
- remote URL;
- latest commit date and subject;
- commit count when cheap;
- tracked languages or key files;
- README summary;
- dirty status without dumping private diffs.

Avoid recursive full-disk grep unless scoped. Exclude `node_modules`, package caches, model weights, `.git`, and vendored dependencies.

## File Guidance

### final.md

Use for the strongest current thesis. It should answer:

- What is the user's current game?
- What is the highest-leverage strategy?
- What should be operated now, not merely built?
- What must be stopped or deprioritized?

### frontier.md

Use for external maps:

- frontier AI/data opportunities;
- scarce data or workflow loops;
- technology shifts;
- markets and leverage points;
- why the user's assets matter against the frontier.

### donelist.md

Use as an evidence-backed ledger, not a resume.

Each major item should include:

- project/repo/product name;
- what was actually done;
- source evidence;
- current status;
- next pressure if relevant.

### memory.md

Use for biographical continuity:

- identity;
- early life;
- education;
- career and founder timeline;
- repeated strengths/weaknesses;
- relationships and constraints;
- decisions that shaped the person.

Do not invent missing years. Use "unknown" or "not yet evidenced".

### soul.md

Use for durable operating instructions:

- temperament;
- values;
- decision rules;
- failure modes;
- boundaries;
- emotional conversion rules;
- agent instructions.

### hobbies.md

Treat hobbies as optionality.

For each hobby:

- evidence of interest;
- why it energizes the person;
- commercial paths;
- smallest paid surface;
- risks or reasons to keep it only as a hobby.

## Privacy Rules

- Private `life-evolve` repos may contain sensitive summaries, but still should avoid raw chat dumps unless explicitly requested.
- Public `life-evolve-skills` repos must contain only generic workflow logic, templates, and redacted examples.
- If copying a private skill into a public repo, remove names, personal events, private URLs, repo scans, and evidence files.

## Output Standard

When finished, report:

- files changed;
- evidence sources used;
- any claims marked as inference;
- repo names and visibility if created;
- push/verification status;
- remaining gaps.
