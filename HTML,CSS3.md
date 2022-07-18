# 7/17 やったこと

- 全体のレイアウト
- トップ

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

# インラインブロック
```go
ブロック要素とインライン要素の特徴を併せ持つインラインブロック要素というものがあります。
インラインブロック要素はインライン要素と同様に横に並びますが、ブロック要素のように幅や高さをもちます。
```

```go
ブロック要素<divタグ>など
要素１
要素２

width,height　指定できる
margin,padding 指定できる
配置　横並び

インラインブロック要素
要素１　要素２

width,height　指定できる
margin,padding 指定できる
配置　横並び

インライン要素　
要素１　要素２

width,height　指定できない
margin,padding 左右のみ指定できる
配置　横並び
```

# display 
```go
<a>タグは初期状態でインライン要素になっていますが、
displayプロパティを使うと、インラインブロック要素に変更することができます。
displayプロパティはblock（ブロック要素）, 
inline-block（インラインブロック要素）, 
inline（インライン要素）を指定することができます。
```
<a href="https://prog-8.com/html/study/2/5#/12">詳しくはこちら</a><br>

# 複数クラスの指定
```go
ボタンのように、「共通の部分があるが、
それぞれ小さい変化をつけたいとき」にはクラスの名前を複数指定すると便利です。
半角スペースで区切って複数のクラスを指定することができます。
```

<a href="https://prog-8.com/html/study/2/5#/13">詳しくはこちら</a><br>

# レイアウト調整
- :hover
```go
カーソルが乗ったときの状態をhoverと言います。
CSSで、セレクタ:hoverとすることで、カーソルが乗ったときのCSSを指定することができます。
```

- border-radius
```go
角を丸めるにはborder-radiusプロパティを用います。
数字が大きいほど角が丸くなります。
```

- text-align
```go
text-alignプロパティを用いることで、テキスト、
インライン要素、インラインブロック要素の配置を指定することができます。
leftで左寄せ、centerで中央揃え、rightで右寄せに設定することができます。
```

# 「margin: 0 auto」と「text-align: center」
```go
要素を中央寄せにする方法として、margin: 0 autoとtext-align: centerを学びましたが、
それらの違いを整理しましょう。
containerクラスのように、広い範囲を囲うようなブロック要素の場合はmarginを、
テキストやボタンのようなインライン要素・インラインブロック要素の場合はtext-alignを使うようにしましょう。
```

<a href="https://prog-8.com/html/study/2/6#/18">詳しくはこちら</a><br>

# アイコン作成
<a href="https://fontawesome.com/">参照</a><br>
