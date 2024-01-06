---
title: "windows PowerShellで問答してもらいながら文章を作って表示する方法"
date: 2024-01-07T01:28:16+09:00
tags: ["PowerShell"]
showToc: true
TocOpen: false
draft: false
ShowBreadCrumbs: true
ShowPostNavLinks: true
UseHugoToc: true
description: "コンソール対話で、一言日記などの元テキストを作成"
---

一言日記などに。  
以下、質問と回答を行い、最終的に表示される形式に整形するスクリプト例。  
これはコンソールでの対話的なプロンプトとして機能する。

```
$title1 =  Read-Host "題名は？"
$content1 =  Read-Host "本文は？"
$todayis = Get-Date -Format "yyyy-MM-dd"
$todayisJapanYoubi= [datetime]::Now
$d=$todayisJapanYoubi.ToString("ddd")
Write-Host "---`n$todayis（$d）`n$title1`n$content1`n---"
```

## chips

- Read-Host

コマンドレットを使用してユーザーに対話的に質問してくれる

- ここでは改行コードを簡素に \`n にしているが、必要に応じて適宜 \`r\`n にする。

- \[datetime\]::Now

現在の日時を取得

- ToString("ddd")

\[datetime\]::Now で取得した現在の日時から、文字列に変換して表示する。  
文字列に変換して表示＝曜日になる。  
"dddd" にすると、「火曜日」など曜日のフルネームになる。