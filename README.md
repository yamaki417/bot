# Line bot開発
## 手順　※後で綺麗にする。
1.STS
以下の手順からSTSをインストール
https://qiita.com/t-shin0hara/items/d60116ab299a4dc8a9d0

2.lombokインストール
https://blog.y-yuki.net/entry/2016/09/11/064316

3.サンプルプロジェクトのインポート 
  3.1 zipファイルを任意のフォルダに解凍
  
  ３.２　STSを起動し解凍したファイルをGradleプロジェクトとしてインポート
  
  3.3 プロジェクトファルを右クリックしてGradle→Gradleプロジェクトのリフレッシュ
  
  ３.４　ビルドエラーが発生していないか確認
  
4. ngrokインストール
  4.1 Windowsは知らんw

## 動作確認
　メッセージAPIは別途連携する。
 
1.bootダッシュボードから起動

2.以下コマンドから実行
　　　ngrok http 8080
   
3.Webhook設定
　　　Line DevelopersのApi設定のWebhook設定に２で実行したURIを設定する。
   例：https://8e96049f63da.ngrok.io + /callback ⇦２で取得したURI＋/callbackで設定

4.botにメッセージを送って動作確認できる。
 
