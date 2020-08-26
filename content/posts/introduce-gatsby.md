---
title: "このブログをGatsbyで作り直した"
date: 2020-05-05T00:00:00+09:00
draft: false
---

例によってタイトルがすべてを語っている。

このブログ、実は自作システムで（といってもフレームワーク使ってるんですけど）今まで[Nuxt.js](https://ja.nuxtjs.org/)という[Vue.js](https://jp.vuejs.org/)系フレームワークを使っていたのですが、微妙に使いづらかったので[Gatsby](https://www.gatsbyjs.org/)に乗り換えました。

GatsbyはNuxt.jsと違ってアプリケーション向けフレームワークではなく、静的に書き出すために使われるものだと思うので（Nuxt.jsみたいな用途だったらNext.js使うと思うので）Nuxt.jsよりは痒いところに手が届かないのかな、と思ったけどそんなことはなさそう。

引き続き[Markdown](https://ja.wikipedia.org/wiki/Markdown)で書いてます。もう[WordPress](https://ja.wordpress.com/)には戻れなさげ。

Gatsbyは[GraphQL](https://graphql.org/)をベースに機能を拡張していく感じで、ブログアプリを一から構築するときにはGraphQLの多少の理解が必要になります。と言ってもそんな難しいことではありません。

画像は[公式ブログテンプレート](https://github.com/gatsbyjs/gatsby-starter-blog)を使えば一旦低画質な画像を表示してロードが完了次第元の画像を出すような遅延ロード的なものを標準で付けてくれるのでページのロード時間も速くなるんじゃないのかなと思います。別にこのサイトは極限まで速さを求めたいわけじゃないんですけど。別に[阿部寛のサイト](http://abehiroshi.la.coocan.jp/)とは戦ってません。

**[GitHubリポジトリ](https://github.com/TinyKitten/Blog)**

---

そういえば43VなLGのスマートテレビを買ったのであとでファーストインプレッションをまとめたいと思います。