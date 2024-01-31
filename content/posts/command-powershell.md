---
title: "よく使う Windows Powershell コマンド"
date: 2024-01-31T18:24:00+09:00
tags: ["PowerShell"]
showToc: true
TocOpen: false
draft: false
ShowBreadCrumbs: true
ShowPostNavLinks: true
UseHugoToc: true
# description: "text"
---

## よく使うのに出てこない

そして使いたいときに限っていくら遡っても履歴が出てこない

- 現在地のディレクトリをエクスプローラーで開く

```Invoke-Item .```

- テキストファイルを、vcodeで開く

```Start-Process code -ArgumentList sample.txt```