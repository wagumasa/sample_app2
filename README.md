# Ruby on Rails チュートリアルのサンプルアプリケーション

これは、次の教材で作られたサンプルアプリケーションです。   
[*Ruby on Rails チュートリアル*](https://railstutorial.jp/)
[Michael Hartl](http://www.michaelhartl.com/) 著

## ライセンス

[Ruby on Rails チュートリアル](https://railstutorial.jp/)内にある
ソースコードはMITライセンスとBeerwareライセンスのもとで公開されています。
詳細は [LICENSE.md](LICENSE.md) をご覧ください。

## 使い方

このアプリケーションを動かす場合は、まずはリポジトリを手元にクローンしてください。
その後、次のコマンドで必要になる RubyGems をインストールします。

```
$ bundle install --without production
```

その後、データベースへのマイグレーションを実行します。

```
$ rails db:migrate
```

最後に、テストを実行してうまく動いているかどうか確認してください。

```
$ rails test
```

テストが無事に通ったら、Railsサーバーを立ち上げる準備が整っているはずです。

```
$ rails server
```

詳しくは、[*Ruby on Rails チュートリアル*](https://railstutorial.jp/)
を参考にしてください。
書き終わったら、この変更をコミットします。

$ git commit -am "Improve the README"
1.4.4でgit commit -a -m "Message"というGitコマンドを実行したことを思い出してください。あのときは “すべてを変更” (-a) オプションとコミットメッセージを追加するオプション (-m) を使いました。上で実行したコマンドで示したように、実はこれらの2つのオプションを1つにまとめてgit commit -am "Message"と実行することができます。

本書では今後もこのサンプルアプリケーションを使い続けるので、Bitbucket上にリポジトリを作成してpushしておくとよいでしょう。

$ git remote add origin git@bitbucket.org:ユーザー名/sample_app.git
$ git push -u origin --all     # リポジト