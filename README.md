# go-heroku

[![Go Report Card](https://goreportcard.com/badge/github.com/genki-sano/go-heroku)](https://goreportcard.com/report/github.com/genki-sano/go-heroku)

## Description

GoでHerokuにデプロイするためのテンプレートです。

詳細は下記で `2020/12/23` に公開予定です。  
https://qiita.com/advent-calendar/2020/go5

## Install

このリポジトリをクローンすれば完了です。

```
# クローン
% git clone https://github.com/genki-sano/go-heroku.git

# アプリのルートディレクトリへ移動
% cd go-heroku
```

## Usage

### ローカル環境を立ち上げる

下記コマンドを入力後に http://localhost:8080 で確認できます。

```
% make up
```

### Herokuにビルドする

```
# herokuログイン
% heroku container:login

# herokuアプリの作成
% heroku create -a go-heroku

# herokuリポジトリをgit登録
% heroku git:remote -a go-heroku

# herokuへデプロイ
% git push heroku master 
```

## Licence

[MIT](https://github.com/genki-sano/go-heroku/blob/main/LICENSE)

## Author

[sunnyG](https://github.com/genki-sano)
