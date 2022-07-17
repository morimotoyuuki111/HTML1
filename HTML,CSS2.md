# 7/15　7/16やったこと

- main
- コンテンツ
- ボーダー
- padding
- margin
- お問合せフォーム

# 詳細
# main
```go
main要素は、「copy-container」、「contents」、「contact-form」の3つの要素で構成されています。
```
<a href="https://prog-8.com/html/study/1/18#/57">mainの構造　詳しくはこちら</a><br>

- <span>要素
```go
文中の一部にCSSを適用させたい場合は、<span>要素で囲みます。
<span>タグにCSSを指定することで、文字の色を一部変えています。
<span>要素の前後には改行は入りません。前後に改行が入るタグと入らないタグに関する
```
  
```go
<h1>
  ようこそ<span>Progate</span> //一部を<span>で囲む
</h1>

span {
  color:#ff0000; //ブラウザには<span>タグで囲んだ部分のみにcssを適用される
}
```
  
# 　ブロック要素　インライン要素
```go
HTMLの要素には、改行される要素と改行されない要素があります。
前後で改行が入り、親要素の幅一杯に広がる要素をブロック要素といいます。
これまで勉強してきた<div>要素や<h1>要素、<p>要素はブロック要素です。
それに対して、<span>要素や<a>要素のように改行されない要素をインライン要素といいます。
```
  
<a href="https://developer.mozilla.org/ja/docs/Web/HTML/Element/blockquote">ブロック要素　詳しくはこちら</a><br>
<a href="https://developer.mozilla.org/ja/docs/Web/HTML/Inline_elements">インライン要素　詳しくはこちら</a><br>

#　ボーダー
```go
要素にボーダー（枠線）をつけるには、borderプロパティを用います。図のように、枠線の太さ、種類、色を指定して使用します。
上下左右すべてに線を付けたい場合はborderとし、特定の場所にのみ付けたい場合は「border-bottom」のように、「border-方向」とします。
他にborder-top、border-left、border-rightなどがあります。
```
  
<a href="https://developer.mozilla.org/ja/docs/Web/CSS/border">border　詳しくはこちら</a><br>
  
# padding margin
```go
これまで余白を作るにはpaddingを使ってきましたが、paddingはborderの内側の余白を作ります。
borderの外側に余白を作りたい場合、marginを用います。
値の指定の方法は、paddingと同じです。
```
<a href="https://developer.mozilla.org/ja/docs/Web/CSS/padding">padding　詳しくはこちら</a><br>
  
<a href="https://developer.mozilla.org/ja/docs/Web/CSS/margin">padding　詳しくはこちら</a><br>
  
- marginをまとめて書く
```go
marginの書き方、個別指定
.logo1 {
  margin-top: 20px;
  margin-right: 10px;
  margin-bottom: 20px;
  margin-left: 10px;
}

marginの書き方、省略形1
.logo1 {
  margin: 20px 10px 20px 10px; //左からtop right bottom left
}
※上から上から順に時計回りに指定
  
marginの書き方,省略形２
.logo1 {
  margin: 20px 10px; //左がtop&bottom 右がright&left
}
※上下、左右の順に指定
```
  
- ボックスモデル
```go
これまで勉強してきたborder, padding, marginは、ボックスモデルという概念に基いています。
HTMLの全ての要素には、border（初期状態では表示されない）があり、その外側の余白はmargin, 内側の余白はpaddingです。
```
<a href="https://developer.mozilla.org/ja/docs/Learn/CSS/Building_blocks/The_box_model">ボックスモデル　詳しくはこちら</a><br>

  
# お問合せフォームのレイアウト
```go
<input>要素は１行のテキスト入力を受け取るための要素です。
<textarea>要素は複数行のテキスト入力を受け取るための要素です。
<input>要素は終了タグが不要な点に注意してください。
```
  
<a href="https://developer.mozilla.org/ja/docs/Web/HTML/Element/input">input要素　詳しくはこちら</a><br>
<a href="https://developer.mozilla.org/ja/docs/Web/HTML/Element/textarea">textarea要素　詳しくはこちら</a><br>
 
- 送信ボタン
```go
 送信ボタンにも、<input>要素を用います。
<input>要素にはtype属性を指定することができ、type属性にsubmitを指定すると、入力欄ではなく送信ボタンになります。
ボタンに表示されるテキストは、日本語のブラウザではデフォルトで「送信」になります。
```
 
```go
ボタンに表示されるテキストを変更することも可能です。
value属性に任意の値を指定することで、ボタンに表示されるテキストを変更することができます。
```
```go 
input type="submit value=""保存"> //ボタンに表示されるテキストを変更
```

# 複数のセレクタに同じCSSを指定する
```go 
 複数のセレクタをコンマ（,）で区切ることで、それらに同じCSSを適用することができます。
これを用いて、<input>要素と<textarea>要素には同じCSSを適用していきましょう。
```
```go 
 html
<form>
  <p>input 要素</p>
  <input>
  <p>textarea　要素</p>
  <textarea></textarea>
  </form>
  
 css
input, textarea { //,コンマで区切って複数のセレクタにCSSを指定
  border: 3px solid #ff0000;
}
```

  
