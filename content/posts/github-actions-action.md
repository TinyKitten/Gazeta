+++
date = 2021-01-26T15:00:00Z
title = "生まれて初めてGitHub ActionsのActionを"

+++
[https://music.apple.com/jp/album/%E8%A3%B8%E8%B6%B3%E3%81%A7summer/1537746569?i=1537746570](https://music.apple.com/jp/album/%E8%A3%B8%E8%B6%B3%E3%81%A7summer/1537746569?i=1537746570 "https://music.apple.com/jp/album/%E8%A3%B8%E8%B6%B3%E3%81%A7summer/1537746569?i=1537746570")

最初のリンクは僕の好きなアーティスト「乃木坂46」のアルバム「生まれてから初めて見た夢」です。

ちょっと必要に迫られてGitHub ActionsのActionを作りました。

何をするためにActionかっつーと指定したフォーマットのJSONを受け取ってCloudflareのDNSの設定を更新するアクションです。

割と最初なので手こずって、累計の作業時間は半日ほど。

まあ、なれてしまえばfetchでCloudflareのAPIを叩くだけなので楽ですね。

コード的に何してるかというと特定のディレクトリのJSONをgrabしてJSON Arrayに変換、Actionに食わせてゴニョゴニョする感じです。

ソースおいておきますね

[https://github.com/TeamKitten/Records](https://github.com/TeamKitten/Records "https://github.com/TeamKitten/Records")

[https://github.com/TeamKitten/cloudflare-dns-action](https://github.com/TeamKitten/cloudflare-dns-action "https://github.com/TeamKitten/cloudflare-dns-action")