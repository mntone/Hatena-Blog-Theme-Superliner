# Hatena-Blog-Theme-Superliner

Superliner は、OSのダークテーマ設定に対応した線を基調とするはてなブログのテーマです。

2021年度自分のブログの雰囲気を一新するために新たに書き起こしたものになります。

# セットアップ

SCSSで開発する場合は、下記の手順でリポジトリのcloneとモジュールのインストールを行います。

## Required Component

- [Node.js](https://nodejs.org/)

## モジュールのインストール

```
$ git clone git@github.com:mntone/Hatena-Blog-Theme-Superliner.git
$ cd Hatena-Blog-Theme-Superliner
$ npm install
```

# 通常のテーマ開発

下記のコマンドで、SCSSファイル変更の監視とコンパイルを行います。

```
$ npm start
```

また、コンパイル後 `build/superliner.css` が作られます。

つづいて、[はてなブログ](https://blog.hatena.ne.jp/)の設定を行います。

1. テーマ検証に使うブログを1つ用意します。
1. 1.で作成したブログの「デザイン設定」にアクセスし、「カスタマイズ」タブの「デザインCSS」の内容を下記に置き換えて保存します。

```
@import url("http://localhost:3000/superliner.css");
```

※ Browsersync のブラウザ自動リロードはサポートしていません。

# 構成

```
superliner/
┣┳ scss/
┃┗┳ lib/
┃ ┗ superliner.scss
┗┳ build/
 ┗ superliner.css
```

# LICENSE

under [MIT license](https://raw.githubusercontent.com/mntone/LICENSE.txt)
