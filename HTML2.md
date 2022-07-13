# 7/13 HTMLの全体構造

# やったこと
- HTMLの全体構造
- HTMLの全体構造(2)
- 全体のレイアウト

<a href="https://developer.mozilla.org/ja/docs/Learn/Getting_started_with_the_web/HTML_basics">HTMLの基本</a><br>

# 詳細
# head要素
```go
<head>要素にはWebページの設定に関する情報を書いていきます。
<head>要素内に記述した内容はWebページには表示されません。
<head>要素には必ず入れる3つの要素がある
```

- head要素の中身
```go
<head>
  <meta charset="utf-8"> //1 文字コード
  <title>Progate</title> // 2 ページタイトル
  <link rel="stylesheet" href="stylesheet.css">　　//3 CSSの読み込み
</head>
```

```go
文字コードを指定することで、ページの文字化けを防ぐことができます。
<meta charset="utf-8">とすることで、そのページの文字コードをUTF-8に
指定することができます。
UTF-8は、HTMLで推奨されている文字コードです。
```
```go
<title>要素は、ページのタイトルを指定します。
<title>要素で指定されたタイトルは、ブラウザのタブ上に現れます。
```

- CSSの読み込み
```go
これまでProgate上では「stylesheet.css」で記述したCSSが結果に反映されていましたが、本来はHTMLの方で読み込む必要があります。
HTMLからCSSを読み込むためには、<link rel="stylesheet">を用います。
<link rel="stylesheet" href="stylesheet.css">のように、href属性で読み込むCSSファイルを指定します。
```

# div要素
```go
レイアウトは<div>要素によって構成していきます。
<div>要素の「div」は「division」の略で、要素をグループ化するために使用されます。
「header」、「main」、「footer」というclass名を持った3つの<div>要素でレイアウトを分割しています。
```
<a href="https://developer.mozilla.org/ja/docs/Web/HTML/Element/div">div要素　詳しくはこちら</a><br>

# エディタの補完機能
```go
ここからはタグを記述する量が増えてきます。
これらを一つ一つ書いていくのは面倒な上、タイプミスもしやすいので、エディタには補完機能があります。
タグ名を入力し、「Tab」キーを押すと終了タグまで補完をしてくれます。
（タグによっては余計なものまで補完される場合もあるので注意してください）
```

<a href="https://developer.mozilla.org/ja/docs/Learn/HTML/Introduction_to_HTML/The_head_metadata_in_HTML">詳しくはこちら</a><br>
