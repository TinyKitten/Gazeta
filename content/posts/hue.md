---
title: "PHILIPSのHueを買ったのでさっそくほめるボタンが押されたときにゲーミングするようにした"
date: 2021-09-16T00:00:00+09:00
draft: false
---

[Hue(YouTube)](https://youtube.com/shorts/Lqt6SIpEsvU?feature=share)

フィリップスHueのスターターセットA60というものを買ってみました。これは電球3本と部屋にある電球を束ねて管理できるようにしてくれるブリッジというものがセットになったもの。

新宿東口のヨドバシカメラで2万円ちょっと。値段的にはだいぶ張る。

なんでこんなのを買ったのかと言うと、いままで[ボクのポートフォリオ](https://tinykitten.me)にあるほめるボタンが押されたときにSlackに通知したりスピーカーから効果音を鳴らすようにしてました。

今回はそれに並行して家の天井照明もゲーミングにしてしまおうという計画です。

セットアップもともとの電球をフルカラーHueに置き換えてブリッジはLANケーブル繋いで電源つける。そしてスマホでセットアップするだけ。

で、このブリッジをRaspberry
Piからぶっ叩いて色を変えれるようにしたいわけで。[このページ](https://qiita.com/tacck/items/67701a6a24003c9021d2)を参考にしました。

もともとのプログラムをちょっと書き換えてほめるボタンが押されたときに1LDKの弊宅がゲーミングしてくれるようになりました。めでたしめでたし。

[実際に動いてるコード](https://github.com/TinyKitten/PhysicalPraiseNotifier)
