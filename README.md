#概要
Markdownテキストからブラウザで動作するHTMLスライドを生成するテンプレート（reveal.js）の使用方法。  
テンプレートの場所やMarkdownの簡単な記法を説明。

- [Demo](http://kotaro-co.github.io/revealjs-template/)
- [reveal.js - The HTML Presentation Framework](http://lab.hakim.se/reveal-js/#/)

#使い方
- 上記ファイル一式をローカルに保存
- index.htmlの該当箇所（Markdownここから　〜　Markdownここまで）にMarkdown記法で文章を書く
- index.htmlをブラウザで開く
以上。

##よく使うタグ
###見出し
```
# Headers - 見出し
## これはH2タグです
### これはH3タグです
#### これはH4タグです
##### これはH5タグです
###### これはH6タグです
```

###リスト
```
- アイテム1
- アイテム2
- アイテム3
```

###リンク
```
https://www.google.co.jp/ →　http,httpsから始まる文字列は自動的にリンクになります。
[Google](https://www.google.co.jp/)
```

###画像
```
![画像](resources/img/nameko.jpg)
```

###ページの分割
```
---
```

##参考）Qiita - Markdown記法 チートシート - Qiita
http://qiita.com/Qiita/items/c686397e4a0f4f11683d

#CSSの変更
これがテーマ用のCSSファイル
```
<link rel="stylesheet" href="resources/css/theme/original.css" id="theme">
```
このCSSを触っても良いし、自分で追加しても良し。

#スライドアニメーションの変更
html下部の以下のオプションを変更
```
transition: Reveal.getQueryHash().transition || 'linear'
```

設定値 | 動き
------------- | -------------
default | パネルが回るような感じ
cube | 箱が回るような感じ
page | ページをパラっとめくるような感じ
concave | パネルが回るような感じ（内側）
zoom | 前後（奥行き方向）に動く感じ
linear | 左右にスライド
fade | フェード
none | 無し

#参考サイト
##Reveal.js、Markdown、Githubでスライドを作成する。 - Qiita
http://qiita.com/budougumi0617/items/19b19019bbe01f86e251