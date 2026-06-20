---
title: "ADR 0002: private寄りとpublic寄りを分ける"
date: 2026-06-20
tags:
  - adr
  - decision
---

同じGarden内でも、個人用メモと公開候補を分けて扱う。

## Decision

`private-patterns/` と `public/` を分け、公開前の編集ルールを[[private-patterns/redaction-policy]]に置く。

## Consequences

公開候補のレビュー導線が作れる一方、リンク先にprivate文脈が漏れない確認が必要。
