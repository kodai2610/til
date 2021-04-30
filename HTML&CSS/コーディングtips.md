## font-sizeの単位について
親のfont-sizeをrem 子のfont-sizeをemで適用。

## sassの利用法
ファイルを分ける

## 余白の単位の使い分け
画面幅によって変わったら％

絶対的なものは%（ロゴ、アイコンなど）

## bootstrap-reboot.cssを使う


## クラスをたくさん振る

保守性の観点からなるべくクラスをつける

## 共通クラスを探し

先に共通部分を見つけ出しクラスを作っておく

## ボタン　

ベーススタイルをbtnクラスで作っておき、変更点を別のクラスで指定

## デイトラ学び

- inline-block ものによって余計な隙間が空きやすい
- imgはblockにする
- li はクラス指定しなくてもいい
- 余計な余白消す　nth-childの利用
-not使う
-左押し　margin-left auto
-”justify-content: space-between;” が簡単ですが、IEでバグが起きる
-キャッチコピーはdivで
-ボタンはdiv + a
-<bg-size> の値は <position> の直後に '/' の文字で区切って含めなければなりません。
-間隔の読み取りはline-heightも踏まえてちょっと小さめにする
-btnはline-heightによる上下中央配置。
-多少のずれはピクセルパーフェクトで直す

















