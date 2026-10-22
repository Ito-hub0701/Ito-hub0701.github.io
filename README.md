# Ito ポートフォリオ

愛知工業大学大学院 経営情報科学研究科に在籍するItoのポートフォリオです。GitHub PagesとJekyllを使い、Markdownで日記を追加できます。

## ファイル構成

- `index.html` — トップページ。最新の日記を3件表示します。
- `index.css` — サイト全体のデザイン
- `face.png` — プロフィールアイコン（70 × 70 px）
- `blog.html` — 日記一覧ページ
- `_config.yml` — Jekyllの設定
- `_layouts/` — 日記一覧と記事ページのレイアウト
- `_posts/` — 日記記事を保存するフォルダー

## 日記を追加する

`_posts`フォルダーに、`YYYY-MM-DD-記事名.md`という名前でMarkdownファイルを作ります。たとえば`2026-10-23-study-note.md`です。

ファイルの先頭に日付とタイトルを書き、その下に本文をMarkdownで記入します。

```markdown
---
title: "今日の学び"
date: 2026-10-23 20:00:00 +0900
---

今日はOpenCVで画像処理を試しました。

## 気づいたこと

- パラメーターを変えると結果がどう変化するか確認した
```

保存してGitHubにコミットすると、日記一覧とトップページの最新記事欄に自動で表示されます。

## GitHub Pagesで公開する

1. `index.html`、`index.css`、`face.png`、`blog.html`、`_config.yml`、`_layouts`、`_posts`をリポジトリのトップ階層にアップロードします。
2. リポジトリの **Settings → Pages** で、公開元を`main`ブランチの`/(root)`に設定します。ブランチから公開する設定ではGitHub PagesがJekyllを使ってサイトをビルドします。
3. 数分後、[https://ito-hub0701.github.io/](https://ito-hub0701.github.io/)を開きます。

Jekyllでは、日付とタイトルを付けたMarkdownファイルを`_posts`に追加して投稿を作れます。詳しくは[GitHub公式ドキュメント](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/adding-content-to-your-github-pages-site-using-jekyll)を参照してください。
