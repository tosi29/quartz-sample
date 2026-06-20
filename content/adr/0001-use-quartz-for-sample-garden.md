---
title: "ADR 0001: サンプルGardenにQuartzを使う"
date: 2026-06-20
tags:
  - adr
  - decision
---

QuartzのWikiリンク、バックリンク、グラフ、検索をまとめて評価するため、サンプルGardenをQuartzで作る。

## Context

AIログや判断メモは階層だけでは探しにくい。リンクネットワークを確認したい。

## Decision

Quartzを採用し、30ページ程度の内容を用意する。

## Consequences

Markdown中心で移植しやすいが、Quartz固有機能への依存は記録する。
