---
title: "Hugo + GitHub Pages を用いたサーバーレスな静的サイトの作り方 1"
date: 2023-06-18T00:08:51+09:00
tags: ["Hugo"]
showToc: true
TocOpen: false
draft: false
ShowBreadCrumbs: true
ShowPostNavLinks: true
UseHugoToc: true
description: "gatsbyから乗り換えたら、記事の新規追加が劇的に楽になりました"
---

## 目標

- 既存の自作ブログをhugoで再構築
 - 現在は `Gatsby Cloud` でホスティング中
 - hugo の方がよりシンプルに保持できそうなので

- hugo で作ったら `GitHub Pages` で公開しよう。

### GitHub Pages で公開

- https://gohugo.io/hosting-and-deployment/hosting-on-github/

hugo公式ドキュメントを参考に。  
`GitHub Actions` を初めて設定した。

- https://qiita.com/ysdyt/items/a581277dd1312a0e83c3

GitHub Pages で公開するためには、hugoの基本構成から少しだけカスタマイズが必要らしい。  
何から何まで参考になりました。感謝。

## 参考にさせていただいたサイト

- https://ie.u-ryukyu.ac.jp/syskan/service/hugo/

- https://github.com/adityatelange/hugo-PaperMod/wiki/Installation#sample-pagemd

取り敢えず、`hugo-PaperMod` なるテーマを使用。  
Installationページを読みながら。

- https://kattsun.dev/posts/how-to-readd-submodules/

add submodule のやり方で何かミスったっぽい。
上記サイトを参考に、解決。

- https://gkzz.dev/posts/add-favicon-with-hugo-papermod/

faviconが認識されない問題

submodule -> themes/PaperMod is empty ?

