# 準備
- `/app`と同じ階層に、`.env`ファイルがないと、動かないと思います。
    - `.env`はデータベースとか、メールとか隠したい情報を格納するやつです。
    - env("名前")で呼び出せます。`/config/database.php`とかに使ってます。


## 状況
とりあえず、新規登録とログインを実装
ログイン： http://it-wiseman.com/auth/login
新規登録： http://it-wiseman.com/auth/register

# ヘイトマン構築メモ

## 構成
- サーバ
    - LAMP

- フレームワーク
    - Laravel5

- 使用ライブラリー
    - Polymer

## 内容
- Laravelを使ってひとつサービスを作ってみる
- 今回は、ヘイトマンというサービスを作ってみたいと思います。
- ついでにマテリアルデザインで構築したいので、Polymerライブラリーを使用する。

### 仕様
- お前が嫌いだを、匿名でやりあうサービス。需要は、わからない。
- hate you しても、誰が押したかはわからないようにする。
- hate you されたユーザーに、なんかメッセージでも送信できるようにしてみよう。


### 必要な機能
- ログイン
- 新規登録
- 一覧
- ヘイトを感じてることを知らせる

### 必要な画面
- ログイン画面
    - email
    - パスワード
    - そのうちFacebook認証

- 新規登録画面
    - email
    - パスワード
    - ユーザー名
    - ユーザーのアイコン

- ユーザー一覧
    - ユーザーのアイコン
    - ユーザー名
    - hate you ボタン
    - 憎まれ数

