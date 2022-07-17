# 7/17 やったこと

- 全体のレイアウト
- トップ
- ヘッダー

# 詳細
- 全体のレイアウト
```go
HTMLの構成は上から　//プロゲートHTML中級参照
header
↓
top
↓
lesson
↓
message
↓
footer
```

# headerとfooter
```go
<div class="header">と<div class="footer">のような、
ヘッダーとフッターのためのタグは非常によく使われるので、
HTMLは<header>と<footer>というタグが用意されています。
<header>, <footer>を使う方が一般的なので、こちらを使いましょう
```
```go
dibとクラス名を用いた方法
<div class="header"></div>

<div class="top-wrapper"></div>

<div class="footer"></div>

<header>と<footer>を用いた方法
<header></header>

<div class="top-wrapper"></div>

<foooter></footer>
```

- 背景画像を指定
<a href="https://prog-8.com/html/study/2/3#/3">詳しくはこちら</a><br>

# 要素を透過される
```go
opacityプロパティを使えば要素を透明にできます。
透明度は0.0(完全に透明) ~ 1.0(完全に不透明)の数値で指定します。
```

# 文字の間隔を指定する
```go
letter-spacingプロパティを用いることで文字の間隔を指定することができます。
```

# ボタン部分を作ろう
```go
ボタンを作っていきます。ボタンは<a>タグで指定します。
しかし<a>タグはインライン要素であり、インライン要素にはwidthやheightが指定できないなど不便な点があります。
これを解決する方法を学びましょう。
```
![Uploading image.png…]()
