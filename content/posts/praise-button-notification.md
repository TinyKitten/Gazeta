---
title: ポートフォリオでほめるボタンが押されたら家のスピーカーが鳴るようにした
date: 2020-10-15T22:21:57+09:00
draft: false
---

{{< youtube eE20rGehDn0 >}}

このブログの存在忘れてました。TinyKitten です。
相変わらず文章が書くのが苦手というか嫌いなので簡素に書いていきます。
[僕のポートフォリオ(TinyKitten.me)](https://tinykitten.me)にはほめるボタンがあって、押されるとカウンターに加算されて僕の Slack に通知が来ます。
Slack だけだとなんか味気ないのでラズパイで通知を受け取る IoT をしてみました。

## 前までのアーキテクチャ

![前までのアーキテクチャ](/img/praise-button-notification/architecture-1.png "前までのアーキテクチャ")

[TinyKitten Portfolio](https://tinykitten.me)のほめるボタンを押されたら Firestore に書き込まれ、Cloud Functions for Firebase で変更を受け取って自分専用の Slack に Webhook で送りつけてました。

それだけだと味気ないので次はこうしてみました:

## 現在稼働しているシステムのアーキテクチャ

![現在稼働しているシステムのアーキテクチャ](/img/praise-button-notification/architecture-2.png "現在稼働しているシステムのアーキテクチャ")

ボタンが押されたときに Cloud Functions for Firebase で Firestore の値を取ってくるのは同じなのですが、新しいアーキテクチャでは一つ動線が増えています。

Slack に対して Webhook するのに加えて、Beebotte に Webhook しています。

Beebotte とは POST されたデータを MQTT に流してくれたりする超すぐれものです（適当）

Beebotte から MQTT で Publish されたデータを Raspberry Pi 上で動いてる Python のプログラムで Subscribe して、データを受け取ったら JR 神戸線のさざなみを流すようにしました。ちなみに、Raspberry Pi である必要はまだありません。

## 今後の展望

とりあえずパトランプ光らせたいですね。
