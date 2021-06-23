---
title: "TrainLCD Image Generatorを作った"
date: 2021-06-24T0:40:00+09:00
draft: false
---

TILやりたいって言ってやってないっすね。きったんです。

作りかけなんですけど、[TrainLCD](https://trainlcd.tinykitten.me)アプリっぽいデザインの画像を生成できる[TrainLCD Image Generator](https://trainlcdgen.tinykitten.me/)を作りました。

実装は特に自慢できる点はなくて、Canvasでゴリゴリ書いてCanvasをbase64化してimgタグのsrcに貼り付けてます。それだけ。

ソースは[ここ](https://github.com/TrainLCD/ImageGenerator)で読んでください。PRs Welcomeです。

今後どう改善していきたいかとかは以下を考えてます：

- TrainLCDアプリと同じようにテーマを選べるようにしたい
- 多言語化対応
- 通過駅対応

あたりですね。完全にTrainLCDアプリそのままって感じのデザインを引っ張ってきたいです。
