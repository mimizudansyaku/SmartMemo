# アプリの公開
このアプリは未完成です。公開はする予定ですが、現在はアクセスすることができません。もうしばらくお待ちください。
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
