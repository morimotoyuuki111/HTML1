# 7/14  

# やったこと
- ヘッダー
- フッター

# 詳細
- ヘッダーの枠組み
```go
ヘッダーには「Progate」のロゴと、ヘッダーメニューのリストがあります。
この二つの部分を、<div>要素を用いてグループ化してみましょう。
```
```go
<div class="header">
  <div class="header-logo">Progate</div>　//ロゴの<div>要素
  <div class="header-list">
    <ul>
    
    </ul>
  </div> //ここまでがヘッダーのリストの<div>要素
</div>
```

```go
Progate //ロゴの<div>

・プログラミング //ヘッダーのリストの<div>
・学べるレッスン
・お問合せ
```

- リストのマークをなくす
```go
<li>要素にlist-styleプロパティを用いてnoneを指定すると、リストの先頭のマークを消すことができます。
基本的に先頭の黒点は必要ないので、消してしまいましょう。
```
```go
CSSに指定ありの場合
<ul>
  <li>黒点なし</li>
  <li>黒点なし</li>
</ul>

css
li {
  list-style: none; //リストのマークをなくす
}

ブラウザでは
黒点なし
黒点なし
```
- ヘッダーの中身を横並びにする
```go
floatプロパティを用いることで、指定した要素を横並びにすることができます。
float: left;を指定すると要素が左から順に横に並びます。
```

<a href="https://developer.mozilla.org/ja/docs/Web/CSS/float">floatプロパティ　詳しくはこちら</a><br>

- 余白の調整
```go
要素に余白を作りたい場合は、paddingを用います。
「padding: 値;」とすると、上下左右すべての方向にその大きさの余白が追加されます。
```

<a href="https://developer.mozilla.org/ja/docs/Web/CSS/padding">padding　詳しくはこちら</a><br>

# フッター
- 入れ子のセレクタ
```go
.header-list」の後にスペースを空けてliと続けると、「header-list」の中の<li>
要素にのみCSSを適用することができます。
これにより、ヘッダーの<li>要素とフッターの<li>要素に別々のCSSを適用することができます。
```
```go
index.html
<div class="header-list">
  <ul>
    <li>ヘッダーのリスト</li>
    <li>ヘッダーのリスト</li>
  </ul>
</div>
<div class="footer-list">
  <ul>
    <li>フッターのリスト</li>
  </ul>
</div>

stylesheet.css
.header-list li{ //header-listの子要素である<li>要素にのみCSSを適用
clolr: #ff0000;
}

```
- float: right
<a href="https://developer.mozilla.org/ja/docs/Web/CSS/float">floatプロパティ　詳しくはこちら</a><br>

- 要素を左右に配置する
```go
Progate ←footer-logo「float:left;」を指定

会社概要
採用　　　　　　　　←fllter-listに「float:right;」を指定
お問合せ　
```
