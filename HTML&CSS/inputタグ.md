##　検索box内虫眼鏡アイコン

html 
~~~
<div class="search_box">
  <input type="serach">
</div>
~~~

css
~~~

.search_box {
  position: relative;    /* 基準値とする */
}

.search_box::before {
  content: "";           /* 疑似要素に必須 */
  width: 10px;           /* アイコンの横幅 */
  height: 160px;          /* アイコンの高さ */
  background: url(./icon.png) no-repeat center center / auto 100%; /* 背景にアイコン画像を配置 */
  display: inline-block; /* 高さを持たせるためにインラインブロック要素にする */
  position: absolute;    /* 相対位置に指定 */
  top: 4px;              /* アイコンの位置。微調整してね */
  left: 5px;             /* アイコンの位置。微調整してね */
}

.search_box input {
  padding: 3px 0 3px 2em; /* アイコンを設置するため左の余白を多めに指定*/
}
~~~

> https://qiita.com/7note/items/86253752adfb95e9bf47
