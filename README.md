# _template
フロントエンド開発をする際の、一番最初に使うテンプレートファイルです。  
_dev 配下で  
```
$ gulp
```
を実行します。

サードパーティ製のファイルを追加した場合は、  
```
$ gulp third
```
を実行します。（監視してません）

## /_dev
開発に使用するファイルを格納します。  
- sass  
SASSファイルを格納します。  
partial は sass/partial に格納します。  
- scripts  
JSファイルを格納します。  
gulpで勝手にまとめます。  
（読み込む場合に順番が必要な場合は gulp ファイルを編集する必要があります。）  
- third  
サードパーティ製のファイルを格納します。  
初期では jQuery v1.8.3、jQuery easing v1.3、jQuery Cookie v1.4.1 が入っています。  
jQuery、jQuery easing、jQuery Cookie の順に読み込みます。  
- views  
htmlファイルを格納します。  
テンプレート用のファイルは views/template に格納します。  
（template配下で _ から始まっているファイル名のファイルはコンパイルしません。）

## /assets
- styles  
SASSがコンパイルされたファイルが格納されます。  
- scripts  
JSが結合、minify化されたファイルが格納されます。  
（サードパーティ製のJSも third.js という名前でここに格納されます。）  