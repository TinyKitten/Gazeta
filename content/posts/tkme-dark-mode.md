---
title: "TinyKitten.meをダークモード対応にした"
date: 2021-06-30T05:00:00+09:00
draft: false
---

最近寝付きが悪くなりました。きったんです。

先程[TinyKitten.me](https://tinykitten.me)のダークモード対応をしました。表示端末がダークモード設定であれば目に優しい色で表示して、ライトモードのときはライトカラーで表示します。要するに今までのままですね。[ちなみに PR はここ](https://github.com/TinyKitten/WebPortfolio/pull/26)

どうやって実装しているかというと、TinyKitten.me は React(Next.js)なので、styled-components を使いました。
[useDarkMode.ts](https://github.com/TinyKitten/WebPortfolio/pull/26/files#diff-61f5f1067506012faa5d33072387b8eb16a7086802a9fb3ffcb1ca25df335ecc)を見ればわかると思いますが、`(prefers-color-scheme: dark)`を見てダークモードと判定できればダークモードであるステートを叩き込んでます。それだけ。簡単。
Custom Hooks で払い出した値は Provider で読んで styled-components のテーマ機構に渡してます。

Custom Hooks にはトグルする機能自体は実装してるので画面的にトグルできるようにすれば完璧だと思います。

締めの言葉が思いつかない...今日職域でワクワクチンチン打ちます。いよいよ 5G 対応の肉体...
