## 文字コード
コンピュータ上で文字を表現するために決められたコードセット。

代表的なコード
-UTF-8（推奨）
-Shift-JIS
-EUC-Jp


##brタグ
Webページのレイアウトのために<br>を使わないようにする。


##imgタグ
alt属性はSEOの観点から重要。必ず記述する


##テーブル

-<table></table>: テーブルを作るタグ
-<tr></tr> : 横一列のデータをまとめる
-<td></td> : セルの要素（データ）
-<th></th> : 表の見出し

##form
<input>属性にあるsizeは入力できる文字数を示す
<textarea>　cols 一行に入力できる文字数　rows　行数
 
##display
block　では、text-alignやvertical-alignが設定できない

inline　では、左右のpadding・marginはok。上下は✕。  text-alignは親要素に。vertical-alignは自身に設定。

none　は表示になるだけで表示が速くなるわけではない→レスポンシブで使う


##flexbox
コンテナにつけるプロパティとアイテムに使うアイテムを分けて理解

Flexアイテムのプロパティ
  -order : 順番を変更 整数
  -flexgrow : コンテナの残りの容量のうちどれだけがそのアイテムに割り当てられるか　
  -flex-shirink :　↑の逆でアイテムの合計のがコンテナよりでかい時どの程度縮ませるか　
  -flex-basis : アイテムの基本幅
  
##margin
-margin-left: auto で右寄せ
-margin-right: auto で左寄せ
-margin: 0 auto で中央寄せ















