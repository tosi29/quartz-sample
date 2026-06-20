---
title: "GitHub Pages docs公開メモ"
date: 2026-06-20
tags:
  - research
---

GitHub PagesのDeploy from a branchで、`main` / `docs`を選ぶ想定のメモです。

## 手順概要

1. `npm ci`
2. `npm run build`
3. 生成された`docs/`を確認
4. Pages設定で`main` branch `/docs`を選択

このPRでは`docs/`はコミット対象外です。
