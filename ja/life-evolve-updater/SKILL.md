---
name: life-evolve-updater-ja
description: 日本語の life-evolve リポジトリを証拠から更新する。final.md, frontier.md, donelist.md, memory.md, soul.md, hobbies.md, progress.md、個人戦略、人生記憶、実績一覧、趣味から副業への可能性を日本語で保守するときに使う。日本語ネイティブのプロンプトで考え、三言語版の論理的一貫性を保つ。
---

# Life Evolve Updater - 日本語

この skill は、日本語の `life-evolve` フォルダ、または多言語 `life-evolve` リポジトリの日本語版を更新するために使う。

## Canonical Files

- `final.md`: 長期戦略と現在の最終仮説。
- `frontier.md`: frontier opportunity、外部地図、leverage point。
- `donelist.md`: 証拠ベースの実績一覧。各 project に完成度を入れる。
- `memory.md`: 人生 timeline、持続的な事実、biographical reconstruction。
- `soul.md`: temperament、values、decision rules、operating constraints。
- `hobbies.md`: 副業化し得る serious interests。
- `progress.md`: repository と update system の完成度。

## Native Prompt

日本語ファイルを更新するときは、日本語で直接考えて書く:

```text
この life-evolve フォルダを証拠から更新する。
事実を守り、推測は推測として明記し、七つのファイルの一貫性を保つ。
その人を一般的な productivity persona に平坦化しない。
shipped work は completion percentage 付きの done-list にする。
趣味は hobby-to-business optionality として評価する。
人生記憶は美談ではなく、運用可能な memory に変換する。
```

## Workflow

1. まず日本語の七つのファイルを読む。
2. 多言語 repo の場合、source-of-record の言語フォルダと照合する。
3. 編集前に証拠を集める:
   - Git repositories と recent commits;
   - README / package metadata;
   - local memory files と notes;
   - user-provided product status;
   - 現在の外部状態が必要な場合だけ public pages。
4. ファイルを system として更新する。
5. `donelist.md` では major project / direction ごとに completion percentage と「なぜ 100% ではないか」を入れる。
6. `progress.md` では repository maturity と project maturity を分ける。
7. commit 前に privacy check を行う。

## Privacy

public repo に raw chats、secrets、credentials、private database dumps、sensitive third-party data を入れない。private repo では、必要で証拠に基づく summary は許容される。

## Completion Percentages

- 0-20%: idea、research、placeholder、early notes。
- 21-40%: prototype または planning repo がある。
- 41-60%: working implementation はあるが product-ready ではない。
- 61-80%: substantial product/system はあるが operation、users、packaging、hardening が必要。
- 81-95%: launched または near-production。残りは operation、scale、monetization、polish。
- 96-100%: users、revenue、retention、maintenance の閉ループ、または intentionally complete artifact。

## Output Standard

変更ファイル、使用した証拠、completion percentage の変更、推測した事実、repo visibility、push status、残りの gap を報告する。
