[![Build Status](https://travis-ci.org/hand-dot/minica.svg?branch=master)](https://travis-ci.org/hand-dot/minica)  
[![Greenkeeper badge](https://badges.greenkeeper.io/hand-dot/minica.svg)](https://greenkeeper.io/)  
## Minica  

### ”思いついたサービスを小さく速くリリースするためのテンプレート”  
  
トップページ・サインアップ・ログイン・アカウント設定・ログアウトページを提供します。
    
   ------------------------------------

技術要素
 * バックエンド - [firebase](https://firebase.google.com/)
 * フロントエンド - [react](https://reactjs.org/)
 * UI - [material-ui](https://material-ui-next.com/)

### アプリ起動

1.レポジトリのクローンとライブラリのダウンロード
```
$ git clone https://github.com/hand-dot/minica.git
$ cd minica
$ npm install
```
  
2.設定ファイルの作成と記入
[`src/`](https://github.com/hand-dot/minica/tree/master/src) 配下に `configs`ディレクトリがあります。  
このディレクトリに存在する firebase.js([Firebase](https://firebase.google.com/)), ga.js([GoogleAnalytics](https://developers.google.com/analytics/)), sentry.js([Sentry](https://sentry.io/welcome/))のアカウント情報を記入してください。  
その他の利用しているサービスについては  
サーバーサイド [Firebase](https://firebase.google.com/)  
チェンジログ [Headway](https://headwayapp.co/)  
エラー解析 [Sentry](https://sentry.io/welcome/)  
アクセス解析 [GoogleAnalytics](https://developers.google.com/analytics/)  
フィードバック [Hot.jar](https://www.hotjar.com/)  
ロードマップ [Trello](https://trello.com/)  
ユーザーコミュニティ [Slack](https://slack.com/)  
ブログ [Medium](https://medium.com/)  
SNS [twitter](https://twitter.com/)  
SNS [facebook](https://www.facebook.com/)  
  
設定ファイルはコミットしないようにminicaディレクトリ上で下記のコマンドを入力して下さい。
```
$ git update-index --skip-worktree src/configs/firebase.js  
$ git update-index --skip-worktree src/configs/ga.js  
$ git update-index --skip-worktree src/configs/sentry.js  
```
  
3.minicaディレクトリ上でアプリを起動
```
$ npm run start
```
