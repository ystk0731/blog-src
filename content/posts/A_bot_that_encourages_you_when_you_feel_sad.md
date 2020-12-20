---
# 記事タイトルの設定
title: "悲しい気分の時に励ましてくれるBot"
# 記事の説明
description : "記事の説明"
# 作成日付の設定
date: "2020-12-17"
# 更新日
lastmod: "2020-12-17"
#アーカイブの設定を作成日付で設定する
archives: [2020/12]
# タグ
tags:  ["LINE", "Bot","GoogleCoudPlatform","CloudNaturalLanguageAPI","NLP"]
# サムネイルの保存場所を/static/thumbnailにする
#thumbnail: "./thumbnail/eye-catch_.jpg"
# 公開終了日付の設定(限定記事以外特に使わない)
#expiryDate: "2020-12-31"
# URLのファイル名部分を変更するパラメータ。基本使わない
#slug: "xxxxx"
# カテゴリ
categories: ["Memo", "備忘録"]
# 目次設定（true=表示、false=非表示）
toc: true
# 下書きモード（true=下書き、false=公開）
draft: true
---

## はじめに

生きてたら誰だって悲しいときはあるよ。人間だもの・・・
<br>
だがしかし、そんな時はだいたい誰も励ましてくれないし、
励まして欲しいアピールしてもウザがられるだけだし、、、
<br>
でも、誰か励ましてよ！！！！励まされたい！！！
<br>
そうだ！ Botに励ましてもらおう！！！
<br/><br/>
ということで、Bot作ります。


## Cloud Function

1. [google cloud](https://console.cloud.google.com/projectselector2/home)


## 発生する費用

- Cloud Functionsの費用
  - 無料枠がある。
  - 料金は下記の項目に応じて決まる。
    - 関数の実行時間
    - 関数の呼び出し回数
    - 関数に対してプロビジョニングされたリソースの数
    - 関数によって送信ネットワークリクエストが作成された場合は別途データ転送料金が発生

- 関数のデプロイの費用
  - 関数は無料枠のないContainerRegistryに保存される
  - 1GBあたり月額約$0.026

- 詳細は[料金](https://cloud.google.com/functions/pricing)参照


https://qiita.com/spre55/items/da2ded18ac4652abb936
## LINE Botの作成


## 構築概要
- BotはLINEを使用して構築
- Botが受け取ったメッセージに対して感情分析を実施
- 感情分析はGoogleCoudPlatformのCloudNaturalLanguage APIを利用
- Botの機能は以下のような感じ。
  - 感情分析の結果、ネガティブなことであれば「元気出しなよ」と励ましてくれる。
  - 感情分析の結果、ポジティブなことであれば「その調子だよ」と励ましてくれる。
- システム概要図は以下のような感じ
  - LINE Developers + GoogleAppScript + CloudNaturalLanguage API






## NLPのAPI有効化



GoogleCloudPlatformのNaturalLanguage APIの簡単なプログラムが作成可能





## aaa

[LINE BOT + Cloud Natural Languageで感情分析してみる ](https://qiita.com/kngsym2018/items/5295d5e7fe7aabc6ab32)

## 参考資料
https://codelabs.developers.google.com/codelabs/cloud-natural-language-python3#2
https://kiosk-dot-codelabs-site.appspot.com/codelabs/cloud-nl-intro-ja/index.html
・[PythonでGoogle Natural Language APIを叩いて感情分析](https://ai-trend.jp/programming/python/google-natural-language-api/)