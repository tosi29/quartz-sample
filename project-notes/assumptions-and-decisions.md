# Assumptions and decisions

## Assumptions

- 評価対象はQuartz v4。
- GitHub Pagesは `main` ブランチの `/docs` を公開する想定。
- サンプルデータは架空で、実秘密情報を含めない。
- 30ページ「程度」を満たすため、MOC、AIログ、技術メモ、ADR、調査メモ、公開候補、private運用例を混在させる。

## Decisions

- `content/feature-tour.md` を確認ガイドの入口にする。
- AIログは `content/ai-logs/`、判断メモは `content/adr/`、公開候補は `content/public/` に分ける。
- `docs/` は `npm run build` で生成できるが、このPRではユーザー指示によりコミットしない。
- Starlight移行可能性を残すため、本文はなるべく標準Markdown中心にする。

## Local verification notes

- `npm run build` should run `npx quartz build -d content -o docs --baseDir quartz-sample`.
- Build output is intentionally ignored by Git in this PR.
