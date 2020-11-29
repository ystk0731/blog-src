---
# 記事タイトルの設定
title: "ブロクの更新方法"
# 記事の説明
description : "忘れそうなのでブログの更新方法メモです。"
# 作成日付の設定
date: "2020-11-29"
# 更新日
lastmod: "2020-11-29"
#アーカイブの設定を作成日付で設定する
archives: [2020/11]
# タグ
tags: ["Hugo", "git"]
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
draft: false
---

# 概要
作成したブログの更新方法を忘れそうなのでメモします。


## 参考ページ

[3分で GitHub にブログを作る (Hugo + GitHub Pages)](https://qiita.com/KoKeCross/items/2b24908f60d235bcc49f)

## 環境構築



```
# 作業ディレクトリ作成
mkdir  hogehoge
cd hogehoge

git clone https://github.com/<UserName>/<RepoName>

cd <RepoName>
git submodule update --init --recursive
```


## Webページ作成

```
# 記事作成
hugo new <DirName>/<ContentName>

# 編集
vi <DirName>/<ContentName>

# 記事をWebページに変換
hugo

```

## gitにアップ
```

# Webページのアップロード
cd public
git add .
git commit -m "author commit"
git push

# 記事のアップロード
cd ..
git add .
git commit -m "author commit"
git push
```

