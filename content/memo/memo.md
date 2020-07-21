---
title: "記事を書くためのメモ【非公開】"
date: 2020-03-01T11:57:22+09:00
archives: "2020/03"
tags: ["ブログ"]
author: toshikun
draft: true
---

# markdown記法

簡単に言えばGo言語で記述された静的サイトジェネレーターです。

インターネットサービスとしてのブログサービスってたくさんあると思います。

FC2とかアメーバとかありますよね。

それを使ってもよかったんですけど、どうせ作るなら独自ドメイン使ってみたかったり

カスタマイズとかしたいな～と思ってHugoというサービスを採用致しました。(hugoおめでとう)

そのhugoというサービスでブログを作成している時にいろいろハマったので

そのエピソードを自分のためにメッモしておきます。




## やったこと

#### ・①アーカイブの表記を年別から月別に変更
このブログに使用しているテーマ(先人に感謝)が[ hugo-blog-jeffprod ](https://themes.gohugo.io/hugo-blog-jeffprod/)というものなんですがこれ、アーカイブの表記が年別なのです。

そのままでもいいんですがtoshikunの好みに合わないので変えていきましょう。

まずテーマの全体を見てみることにしました。

`C:\hugo\newblog\themes\hugo-blog-jeffprod\layouts\index.html`


この`index.html`にいろいろ書いてありそうなので見てみます。

と中身をみてアーカイブに関係ありそうなものを見つけました。
```
 {{ partial "widget-archives.html" . }} 
```
`widget-archives.html`っていうファイルを呼び出しているっぽいですね。

こいつの中身を見てみましょうか。

>partial "widget-archives.html"

とあるので*partial*ってきっと関数なんだろうな。

`C:\hugo\newblog\themes\hugo-blog-jeffprod\layouts`配下を見てみます。


{{< img src="/img/test.png" title="test1" >}}
{{< img src="/post/2020/03/0316/img1.png" title="test2" >}}


#### ・②アーカイブの表記を年別から月別に変更<br>
ヘッダーの画像をデフォルトから自分の用意したものに変更

## hugoの導入手順

### ①hugoのインストール
hugoのインストールからしていきましょう。

[ここに](https://github.com/gohugoio/hugo/releases)アクセスします。




