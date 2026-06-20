---
title: "ADR 0003: GitHub Pages向けにdocsへ出力する"
date: 2026-06-20
tags:
  - adr
  - decision
---

`main`ブランチの`/docs`をGitHub Pagesで公開する想定に合わせる。

## Decision

ビルドコマンドは `npx quartz build -d content -o docs` とする。

## Note

このPRでは依頼により`docs/`の中身はコミットしない。ローカルで生成確認のみ行う。
