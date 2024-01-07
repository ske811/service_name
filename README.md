# [PremiaTalk(仮)]

# サービス概要

- プレミアリーグ（欧州サッカー）を試合後に楽しむことに特化したサービス

# 想定されるユーザー層

- プレミアリーグの試合後の感想を投稿したい人 / それらの感想を見たい人
- 10〜20代の層が視聴者層からも多いと思われる

# サービスコンセプト

### なぜそのサービスを作ろうと思ったのか

- 元々プレミアリーグを観戦することが趣味でして
試合観戦はもちろん、試合後に他の方の感想を見るのがもう一つの楽しみとなっており
youtubeのハイライト動画のコメント欄やSNSでの投稿など色々な所で拝見している一方
様々な箇所で感想が投稿されている分、感想の分散化と調べる手間がある点
- また試合後の感想や試合結果や選手スタッツをひとつのプラットフォームで行えるサービスがあると便利だなと思い作成しようと思いました。

### サービスの差別化ポイント・推しポイント

- 試合後の感想や試合結果や選手スタッツを一つのプラットフォームでまとめられている点
- 投票ランキングシステムでその試合のMVPやベストプレーをユーザー間で決めることによるコミュニティの活性化
- 自分で調べた範囲ではありますが、SNS機能と簡易的に試合結果等を確認できるアプリケーションがなかった点

### サービスの利用イメージ

- 試合後の一覧画面: プラットフォームにログインすると、当日のプレミアリーグ試合結果や選手スタッツが一覧で表示される。ユーザーは気になる試合を選び、詳細情報にアクセスできる。
- 感想投稿: ユーザーは試合後に感想やコメントを投稿できる。テキストだけでなく画像投稿
- ファン投票: ユーザーは試合のMVPやベストプレーを投票し、ランキングはリアルタイムで更新され、ユーザーが誰が最も印象的だと思っているかが分かる機能
- ニュースフィード: プレミアリーグやクラブに関する最新のニュースがユーザーのフィードに表示され、タイムライン上でスクロールできるようにする。

# 機能実装

### MVP

- 会員登録機能
- ログイン機能
- 投稿機能
- コメント機能
- いいね機能
- タグ機能
- **検索機能**
- チャット機能
- ファン投票機能
- 試合結果の表示機能(API-Football )
- ニュースフィード（NewsAPI）
- ユーザープロフィールの拡張

### 本リリース

- 詳細情報ページ(API-Football )
- 画像投稿機能
- 通知機能
- レコメンド

# 機能の実装方針予定

- API-Football (試合日程、試合結果、順位表)
- NewsAPI：サッカー関連のトピックを取得
- 通知機能
    - 投稿に対するリアクション通知: 自分の投稿にいいねやコメントがついたとき、通知が届く
- レコメンド
    - 興味タグの利用：投稿には興味タグを付けておき、ユーザーが特定の興味を持つタグに基づいてレコメンドを行う
    - 人気の投稿：他のユーザーが注目しているコンテンツを推薦
- 画像投稿機能

# 技術選定

- JavaScript
- Ruby on Rails
- PostgreSQL
- WebSocket