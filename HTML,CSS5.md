# 7/19 やったこと

- メッセージ部分
- フッター
- ヘッダー

# 詳細
# 立体的なボタン
```go
ボックスに影を付けるためにはbox-shadowプロパティを用います。
```
<a href="https://developer.mozilla.org/ja/docs/Web/CSS/box-shadow">box-shadow 詳しくはこちら</a><br>

- cursor
```go
cursorプロパティを用いることでマウスのカーソルが要素に乗ったときのカーソルの形を変えることができます。
タグによってcursorが初期状態で設定されているものもある
```
<a href="https://prog-8.com/html/study/2/15#/43">cursor 詳しくはこちら</a><br>

# クリック時に変化
```go
セレクタにactiveを用いることで、要素がクリックされている間だけCSSを適用することができます。
セレクタ:activeというように指定します。
```
<a href="https://developer.mozilla.org/ja/docs/Web/CSS/:active">:active 詳しくはこちら</a><br>

# CSSを打ち消そう
```go
box-shadow: none;とすると、影を消すことが出来ます。
このように多くのプロパティはnoneを指定することによって消すことができます
```

# position: relative;による位置の変更
```go
前回position: relative;はposition: absolute;の基準位置を決めるために使っていましたが、要素の位置を変更するためにも使うことが出来ます。
position: relative;をtopやleftと併用すると、その要素を本来の位置からずらせます。
```

# ボタンをへこまそう
```go
クリック時に、以下の処理をすることによって、ボタンがへこんで見えるようになります。
・box-shadowをnoneにする
・position: relative;とtopによって影の分だけ位置を下げる
```

# フッター
```go
footerの中にcontainerで
imgとpがある
```

# ヘッダー
- 要素の重なり順
```go
positionを使用すると要素の重なりが生じます。
レッスン紹介部分とヘッダーが重なった時に、ヘッダーが隠れてしまいます。
```

<a href="https://developer.mozilla.org/ja/docs/Web/CSS/position">position 詳しくはこちら</a><br>

# 要素の重なりの順序をする
```go
z-indexプロパティは、要素の重なりの順序を指定する際に使用します。
z-indexは整数値で指定し、値が大きいほど上に表示されます。
z-indexプロパティは必ずpositionプロパティと併用する必要があるので、注意しましょう。
```

<a href="https://developer.mozilla.org/ja/docs/Web/CSS/z-index">z-index 詳しくはこちら</a><br>
