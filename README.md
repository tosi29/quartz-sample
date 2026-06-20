# Quartz sample garden

このリポジトリは、Quartz が「自分用のAI会話ログ・技術メモ・調査メモ・判断メモを蓄積し、将来的に一部を他人にも見せる」用途に合うかを評価するためのサンプルサイトです。

## 作ったもの

- Quartz v4 ベースのサイト本体
- `content/` 配下のサンプルコンテンツ（30ページ程度）
- `Feature Tour / 機能確認ガイド`
- Wikiリンク、バックリンク、タグ、Graph、MOC、検索、画像、表、長文/短文メモ、AIログ、ADR、技術調査メモの確認材料
- `project-notes/` 配下の仮定・設計判断メモ

## ローカル起動

```bash
npm ci
npm run dev
```

既定では http://localhost:8080/quartz-sample/ で確認します。

## ビルド

```bash
npm run build
```

ビルド成果物は `docs/` に出力されます。

## GitHub Pagesで `docs/` を公開する方法

1. GitHubのリポジトリ設定を開く。
2. **Pages** を選ぶ。
3. Source を **Deploy from a branch** にする。
4. Branch を `main`、folder を `/docs` にする。
5. `npm run build` で生成した `docs/` をコミットしてpushする運用にする。

## ソースとビルド成果物の関係

- 入力: `content/`, `quartz.config.ts`, `quartz.layout.ts`, `quartz/`
- 出力: `docs/`
- `docs/` はGitHub Pages公開用の生成物です。

## ビルド成果物のコミット方針

Issue本文では `docs/` を生成物コミットとして分ける方針でしたが、このPRでは依頼により `docs/` の中身はコミットしません。必要な場合は、レビュー後に別コミットで `docs/` だけを追加してください。

## 人間が確認すべき主な機能

- `content/feature-tour.md` から各ページへ移動できるか
- WikiリンクとBacklinksが期待通りに表示されるか
- GraphでAIログ、MOC、ADR、公開ページの関係が見えるか
- `RAG`, `ADR`, `GitHub Pages`, `private` などで検索できるか
- 30ページ程度でもExplorerで迷子になりにくいか
- `public/` と `private-patterns/` の分離が運用イメージに合うか

## 既知の制約

- サンプル内のAIログ・会議メモは評価用の架空データです。
- `private-patterns/` は非公開運用の例であり、実秘密情報は含みません。
- Quartz固有のWikiリンクを使っているため、Astro Starlightへ移行する場合はリンク変換が必要です。
- このPRでは `docs/` をコミットしないため、GitHub Pagesで公開するにはローカルまたはCIでビルド成果物を追加する必要があります。
