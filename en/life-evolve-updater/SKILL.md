---
name: life-evolve-updater-en
description: Update an English life-evolve repository from evidence. Use when the user asks to maintain final.md, frontier.md, donelist.md, memory.md, soul.md, hobbies.md, progress.md, personal strategy, life history, shipped work, or hobby-to-business surfaces in English. The skill uses English-native prompts and keeps multilingual editions logically aligned.
---

# Life Evolve Updater - English

Use this skill to maintain an English `life-evolve` folder or an English mirror of a multilingual life-evolve repository.

## Canonical Files

- `final.md`: long-horizon strategy and current thesis.
- `frontier.md`: frontier opportunities, external maps, and leverage points.
- `donelist.md`: evidence-backed work record with per-project completion percentages.
- `memory.md`: life timeline, durable facts, and biographical reconstruction.
- `soul.md`: temperament, values, decision rules, and operating constraints.
- `hobbies.md`: serious interests that may become side businesses.
- `progress.md`: repository and update-system completion tracking.

## Native Prompt

When updating English files, think and write directly in English:

```text
Update this life-evolve folder from evidence.
Preserve facts, mark inference, and keep the seven files consistent.
Do not make the person generic.
Turn shipped work into a done-list with completion percentages.
Turn interests into hobby-to-business optionality.
Turn personal history into operational memory, not biography theater.
```

## Workflow

1. Read all seven English files first.
2. If this is a multilingual repo, compare against the source-of-record language folder.
3. Gather evidence before editing:
   - Git repositories and recent commits;
   - README/package metadata;
   - local memory files and notes;
   - user-provided product status;
   - public pages only when current external status matters.
4. Update the files as a system.
5. In `donelist.md`, every major project or direction must have a completion percentage and a reason why it is not 100%.
6. In `progress.md`, track repository maturity separately from project maturity.
7. Run a privacy check before committing.

## Privacy

Do not commit raw chats, secrets, credentials, private database dumps, or sensitive third-party data into public repositories. Summaries are acceptable in private repositories when they are necessary and evidence-backed.

## Completion Percentages

Use this scale:

- 0-20%: idea, research, placeholder, or early notes.
- 21-40%: prototype or planning repo exists.
- 41-60%: working implementation exists, but not product-ready.
- 61-80%: substantial product/system built; needs operation, users, packaging, or hardening.
- 81-95%: launched or near-production; remaining gap is operation, scale, monetization, or polish.
- 96-100%: closed loop with users, revenue, retention, and maintenance, or intentionally complete artifact.

## Output Standard

Report changed files, evidence sources, completion percentage changes, any inferred facts, repo visibility, push status, and remaining gaps.
