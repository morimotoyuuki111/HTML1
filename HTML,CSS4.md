# 7/18 やったこと

- ヘッダー
- レッスン

# 詳細
# ヘッダーのレイアウト

```go
ヘッダー部分
headerの中にcontainerがあり
containerの中にheader-left　ロゴ画像　header-right　ログインリンク
```

# opacityとrgba
```go
これまで要素を透明にするにはopacityを用いてきました。
しかし、opacityには要素の中身全てを透明にするという性質があります。
背景色のみを透明にするには、というものを使う必要があります。
```
- rgb
```go
rgbaを学ぶには、まずrgbというものを理解する必要があります。
rgbは色の指定の仕方の1つで、3つの値の組み合わせで表示する色を決めます。
色を指定するときは今まで使用してきた#ffffffのような記法を使ってもrgbを使っても構いません。
```
```go
.box1 {
  background-color: rgb(255,147,30):
}

.box2 {
  background-color: #ff931e;
}

上記二つのコードは同じ色
```

- rgba
```go
色を透明にしたいときは色をrgbaで指定します。
rgbaは4つの値をコンマ（,）区切りで入れます。
4つ目の値が透明にする度合いで、0 ~ 1の数値で指定します（値が小さいほど透明になります）。
opacityプロパティは要素全体を透過させますが、rgbaを使うとその色だけを透明にすることが出来ます。
```
<a href="http://www.htmq.com/css3/rgba.shtml">rgba 詳しくはこちら</a><br>

# transition
```go
transitionを使うとアニメーションをつけることができます。
「変化の対象」や、「変化にかかる時間」などを指定できます。
「変化の対象」にはcolorなどのプロパティを指定しますが、allを指定すると全てのプロパティに適用出来ます。
transitionは多くの場合hoverと組み合わせて使います。
```

<a href="https://developer.mozilla.org/ja/docs/Web/CSS/transition">transition 詳しくはこちら</a><br>

# 行間を指定する
```go
line-heightプロパティを使うと、行の高さを指定することができます。
値が大きいほど行間が大きくなります。
```

<a href="https://developer.mozilla.org/ja/docs/Web/CSS/line-height">line-height 詳しくはこちら</a><br>

- line-heightと縦の中央寄せ
```go
line-heightプロパティは本来行間を調整するためのプロパティですが、要素の縦方向の中央に文字を配置するのにも使えます。
line-heightプロパティの「高さの中心」に文字が配置されるため、要素の高さとline-heightプロパティを同じ値にすると、文字がちょうど中央に配置されるようになります。
```

# aタグをクリックできる範囲
```go
<a>タグはインライン要素なので、中身のテキストの部分しか大きさを持ちません。
その結果、<a>タグをクリックできる範囲はテキストの部分だけになってしまいます。
<a>タグをブロック要素にすると、大きさが親要素いっぱいに広がるので、全体をクリックできるようになります。

インライン要素はテキスト範囲以外クリックできない。
ブロック要素はボタン全体をクリックできる
```

# レッスンのレイアウト
```go
lesson-wrapperの中に
continuerがあり次がheadingがあり
その中にlessons
```
# 文字の太さを指定する
```go
font-weightプロパティを用いると文字の太さを変更することができます。
normalまたはboldを指定します。
<h1>~<h6>の要素は初期状態でfont-weight: bold;となっているので、
font-weight: normal;と指定すれば文字が細くなります。
```
<a href="https://developer.mozilla.org/ja/docs/Web/CSS/font-weight">font-weight 詳しくはこちら</a><br>

# 相対的な大きさの指定
```go
css
ボックスのwidthやheightをpxではなく%で指定すると、
親要素に対してどのくらいの幅や高さを持つか指定することができます。
```

# position: absolute;
```go
HTMLの要素同士は通常重なって表示されることはありませんが、
position: absolute;を使うと、要素同士を重ねて表示することが出来ます。
サイト全体の左上部分を基準とし、そこからの位置をtopとleftを用いて指定します。
また、rightやbottomを併用することも可能です。
```

<a href="https://developer.mozilla.org/ja/docs/Web/CSS/position">position 詳しくはこちら</a><br>
