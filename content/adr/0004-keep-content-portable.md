---
title: "ADR 0004: Markdownを移植しやすく保つ"
date: 2026-06-20
tags:
  - adr
  - decision
---

将来的なAstro Starlight移行を考え、本文は標準的なMarkdownを中心にする。

## Decision

Quartz固有のWikiリンクは使うが、過度なカスタムコンポーネントは避ける。

## Consequences

移行時はWikiリンク変換が必要。ただし内容そのものは流用しやすい。
