---
title: "Feature Tour / 機能確認ガイド"
date: 2026-06-20
tags:
  - feature-tour
  - moc
---

このページは、人間がQuartzの使い勝手を確認するためのチェックリストです。

| 確認観点                 | 見るページ                                | 期待して見ること                          |
| ------------------------ | ----------------------------------------- | ----------------------------------------- |
| Wikiリンクとバックリンク | [[notes/wiki-link-patterns]]              | `[[...]]` の相互参照、右ペインのBacklinks |
| タグ運用                 | [[notes/tag-taxonomy]]                    | `#ai-log` や `#adr` の一覧性              |
| グラフ                   | [[mocs/ai-memory-moc]]                    | AIログ・ADR・公開メモのつながり           |
| 検索                     | [[research/vector-search-evaluation]]     | 専門語でのヒット感                        |
| 長文メモ                 | [[research/quartz-vs-starlight]]          | 目次、スクロール、読書体験                |
| 短文メモ                 | [[notes/inbox-capture-rules]]             | 小さい断片の扱いやすさ                    |
| AI会話ログ               | [[ai-logs/2026-06-18-agent-debugging]]    | 生ログから要点へ辿れるか                  |
| ADR                      | [[adr/0001-use-quartz-for-sample-garden]] | 判断メモの保管に向くか                    |
| 図表・画像               | [[notes/knowledge-pipeline-diagram]]      | アセット表示と本文との関係                |
| public/private分離       | [[private-patterns/redaction-policy]]     | 公開前の伏せ字ルール                      |

## 評価の進め方

1. まず左ペインのExplorerで30ページ前後の迷子感を見る。
2. 検索で `RAG`, `ADR`, `公開`, `private` を試す。
3. Graphで `AIログ → 抽出メモ → ADR → 公開ページ` の線が見えるか確認する。
