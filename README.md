# アプリのURL
https://smart-memo.herokuapp.com/
# アプリの説明(2020/8/24現在)
メモの新規投稿、変更、削除ができます。ユーザ名やメモ内容などはMongoDBに記録されます。ログイン機能がありますが、現在はTwitterからのログインのみとなります。本来はメモの内容を投稿者とそのフレンドにのみ閲覧を許可する予定ですが、現在は全てのユーザに内容が見えてしまっています（掲示板のようなものです）。このアプリは公開されており現在正常に動作していますが、まだ未完成となっています。
# アプリの動作環境
- Node.js(使用言語)
- heroku（サーバ）
- mLab:MongoDB(データベース)
- TwitterAPI(ログイン用)
# 起動する順番
Node.jsとnpm, MongoDBを導入済みの前提
## 1.外部モジュールをインストール
```
sudo npm install
```
## 2.DBファイルを保存するためのフォルダを作成
```
mkdir db
```
## 3.MongoDBを起動
```
sudo mongod --dbpath db
```
## 4.アプリを起動する
```
nodo app.js
```
## LessファイルをCSSファイルに変換
```
./node_modules/less/bin/lessc less/app.less css/app.css
```
