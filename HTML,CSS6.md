# 7/20 やったこと

- メディアクエリ
- レスポンシブデザイン

# 詳細
# メディアクリエリの書き方
```go
メディアクエリは、@media (条件) { .... }という様に書きます。
指定された条件が当てはまるときにのみ{ }内のCSSが適用されます。
```

```go
＠media (max-width: 1000px ){ //max-width: 1000pxはCSSを適用したい最大幅　１０００pxの後ろはセミコロンはつけない

/*1000px 以下の時に適用したいCSSを記述*/
}
```

# max-widthとmin-width
```go
メディアクエリの条件には、max-width(最大幅)、またはmin-width(最小幅)を指定できます。
max-width: ◯◯pxと指定すると、画面幅が◯◯px以下の時にCSSを適用できます。min-widthはその反対となります。
```

<a href="https://developer.mozilla.org/ja/docs/Web/CSS/max-width">max-width 詳しくはこちら</a><br>
<a href="https://developer.mozilla.org/ja/docs/Web/CSS/min-width">min-width 詳しくはこちら</a><br>

- ブレイクポイント
```go
max-width: ◯◯px（またはmin-width: ◯◯px）のようにメディアクエリの条件を指定するとき、「◯◯px」の部分をブレイクポイントと呼びます。
今回はスマートフォンの画面幅は670px以下、タブレットの画面幅は670px ~ 1000pxと想定して、ブレイクポイントを設定しましょう。
```
<a href="https://developer.mozilla.org/ja/search?q=%E3%83%96%E3%83%AC%E3%82%A4%E3%82%AF%E3%83%9D%E3%82%A4%E3%83%B3%E3%83%88">ブレイクポイント 詳しくはこちら</a><br>

# viewportの設定
```go
レスポンシブデザインを適用する準備として、<head>タグ内にviewportを設定しましょう。
viewportを設定しないと、スマートフォンやタブレットでの閲覧時にメディアクエリが正しく機能しません。
ただし、ここでviewportの中身の書き方を暗記する必要はありません。
```

<a href="https://shu-sait.com/viewport-setting/">viewport 詳しくはこちら</a><br>

# responsive.cssの読み込み
- タブレット向けのレイアウトを作ってみよう
```go
stylesheet.cssにメディアクエリ用のCSSを記述しても問題ありませんが、
整理しやすいように今回はCSSファイルを分割し、responsive.cssにメディアクエリ用のCSSを記述していきます。
このresponsive.cssを読み込む際には、必ずviewportよりも下の行に記述するようにしましょう。
```
<a href="https://www.fom.fujitsu.com/goods/pdf/webcreator/fpt1418-2.pdf">responsive.cssの読み込み 詳しくはこちら</a><br>

# floatと親要素の高さ
```go
通常、親要素の高さは子要素を包む高さとなります。
しかし、子要素が全てfloatの時、親要素の高さは0となってしまうという性質があります。
これは、floatは「浮いている」という意味で、親要素から見るとfloatの子要素は存在しないように見えるからです。
```
# floatの解除
```go
子要素が全てfloatでも、親要素が高さを持つように設定してみましょう。
floatはclear: left;で「浮いている」状態を解除できます。
ここではclear: left;を適用するためだけの空のタグを用意しましょう。
空タグとclearでfloatを解除するのはよく使うテクニックなので、覚えておくようにしましょう。
```

# 要素の表示/非表示
```go
メニューアイコンはデフォルトでは非表示にし、
画面幅が670px以下（スマートフォンサイズ）の時にのみ表示されるようにします。
要素を非表示にするにはdisplay: none;を用います。
非表示にした要素を表示させる時は、display: block;を用いて表示します。
```
<a href="https://web-de-asobo.net/2022/04/15/element-hide/">要素の表示/非表示の読み込み 詳しくはこちら</a><br>

