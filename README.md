Scala Conference in Japan 2013
===========================================================

この Project は Scala Conference in Japan 2013 の管理で利用します。

情報は[Wiki](https://github.com/scalajp/scalaconf-jp-2013/wiki)に集約。


## www.scalaconf.jp の更新

ウェブサイトを複数ページに対応させるにあたり、Jekyll を使って作業をするようにします。

### セットアップ

Mac OS X でのみ確認しています（Windows での確認者求む）。

まず rbenv か RVM で Ruby のセットアップをします。

Jekyll が必要です。

```
gem install bundler
bundle install
```

サーバを起動してブラウザから http://localhost:4000/ にアクセスすると確認できます。

```
jekyll --server
```

静的ファイルは _site 配下に生成されます。

### 使っているもの

- Jekyll

https://github.com/mojombo/jekyll

- Jekyll-Bootstrap

とりあえず不要なものは削っています。

http://jekyllbootstrap.com/

参考:

http://d.hatena.ne.jp/yuum3/20120620/1340180894

http://krakenbeal.blogspot.jp/2012/05/ruby-jekyll-jekyll-bootstrap.html

### 基本的な設定

_config.yml が基本設定です。

### レイアウト

_layout から _include/themes/twitter を参照しています。

ファイルは assets の下に置きます。

### 新しいページの追加

```
rake page name="en/index.md"
rake page name="en/index.html"
```
のようにして生成します。

### 公開

Jekyll は _site 配下に静的コンテンツを出力します。

本番にはこのディレクトリ配下のファイルを転送して公開します。


### 困ったら

特に詳しい訳ではないですが、Jekyll を導入した瀬良（@seratch）に連絡をください。

co-meeting やメール（seratch@gmail.com）でどうぞ。

