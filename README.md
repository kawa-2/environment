# README

## 第1章

#### 学習事項

* RailsとRubyのバージョンが合わないと動かない為、実行するPJによってバージョンを確認する<br>
今回、Railsバージョン5.1.6を動かすには、rubyバージョン2.3.1では動かなかった為、2.6.5をインストール
* Gemfileの内容を変更したらbundle install の実行を忘れずに。
* rails new hello_app :Railsアプリ構造でhello_appというディレクトリを生成することができる。
* rails serverでRailsサーバーを実行し、http://localhost:3000/ で確認。
* Herokuへpushすれば同時にデプロイされる（デプロイコマンド: git push heroku master）

#### 苦戦したところ

* 開発環境づくりに苦戦。
Dockerで環境構築は初心者にはハードルが高く感じてしまい断念。（今後Dockerでの環境構築をできるようにする）<br>
最終的にローカルで環境構築を行った。

* ローカル環境構築手順：https://railsgirls.jp/install
brew install yarn を実行
→linkを貼る権限がないとのことでエラーがでる。（/usr/local/include に書き込み権限がない）
→権限を変更しようとしましたがそもそも変更の権限がないため、新たにディレクトリを作成し書き込み可能にした。
```
sudo mkdir /usr/local/include
sudo chmod 775 /usr/local/include
sudo chown <user名>:admin /usr/local/include
```

#### メモ

Heroku https://rails-environment.herokuapp.com/
