## gitの使い方ドキュメント
***


### 初期設定
```
以下でgitのアカウント上をローカルに登録する
git config --global user.name "XXXX"

git config --global user.email "XXXX@hogehoge.com"
```



### gitを使うときのあいず
- gitを使う時に必ず最初に1回以下のコードを叩いて実行する
  - ※一番上のディレクトリで宣言する

``
git init
``

### リモートリポジトリを登録する
```
git remote add origin ここにリポジトリのURL

!URLを変更したい時
git remote set-url origin URL
```


### ローカルのコードをリモートリポジトリに送信する。
```
変更内容を追加する。(最後のドットは、全てのファイルという意味)
git add .

変更内容を確定する。(-m 後ろに変更内容のメッセージを入れるということ。)
git commit -m 'ここにコメント'

リポートリポジトリに変更内容を送信する
git push origin main

※チーム開発の時はブランチとか切るので今はパス
```


### リモートからコードをとってくる
```
git clone ここにリポジトリのURL
```

