---
title:  "Jekyllのローカルテスト"
date:   2025-09-13 08:27:31 +0900
categories: 環境構築 開発
tags: Jekyll
---

## パッケージやライブラリのインストール
以下のコマンドを実行し、パッケージやライブラリをインストールする。
```bash
bundle install
```

## ローカルでビルド・サイト実行
以下のコマンドを実行し、ビルド・サイト実行する。
```bash
bundle exec jekyll serve
```
※ドラフトのページを確認したい場合、オプション```--drafts```を追加する。

## パッケージやライブラリの更新
Gemfileの更新などを行った場合、以下のコマンドでパッケージやライブラリを更新する。
```bash
bundle update
```

## 参考サイト
- [Jekyll を使用して GitHub Pages サイトをローカルでテストする](https://docs.github.com/ja/pages/setting-up-a-github-pages-site-with-jekyll/testing-your-github-pages-site-locally-with-jekyll){:target="_blank"}
