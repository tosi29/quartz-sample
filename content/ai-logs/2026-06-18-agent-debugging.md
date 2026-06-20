---
title: "AIエージェントのデバッグログ例"
date: 2026-06-20
tags:
  - ai-log
  - raw
---

HermesでCI失敗を追跡した想定ログ。失敗ログを読み、仮説を立て、最小修正で再実行する流れを残す。

## 抜粋

> User: テストが落ちている理由を調べて。
> Agent: まず失敗したジョブ名とログ末尾を確認します。

## 知識化候補

- 再現コマンドはPR本文にも残す。
- 「修正したつもり」ではなく、実行結果を残す。

関連: [[notes/ai-log-to-note-workflow]], [[notes/backlink-review-routine]]
