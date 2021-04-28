### html

~~~
<body>
    <div class="content">
        <a class="js-modal-open" href="" data-target="modal01">クリックでモーダル1を表示</a><br>
        <a class="js-modal-open" href="" data-target="modal02">クリックでモーダル2を表示</a>
    </div>
    <div id="modal01" class="modal js-modal">
        <div class="modal__bg js-modal-close"></div>
        <div class="modal__content">
            <p>1つ目モーダルウィンドウです。ここにモーダルウィンドウで表示したいコンテンツを入れます。モーダルウィンドウを閉じる場合は下の「閉じる」をクリックするか、背景の黒い部分をクリックしても閉じることができます。</p>
            <a class="js-modal-close" href="">閉じる</a>
        </div><!--modal__inner-->
    </div><!--modal-->
    <div id="modal02" class="modal js-modal">
        <div class="modal__bg js-modal-close"></div>
        <div class="modal__content">
            <p>2つ目モーダルウィンドウです。ここにモーダルウィンドウで表示したいコンテンツを入れます。モーダルウィンドウを閉じる場合は下の「閉じる」をクリックするか、背景の黒い部分をクリックしても閉じることができます。</p>
            <a class="js-modal-close" href="">閉じる</a>
        </div><!--modal__inner-->
    </div><!--modal-->
</body>
~~~


### css

~~~

*{
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}
.content{
    margin: 0 auto;
    padding: 40px;
}
.modal{
    display: none;
    height: 100vh;
    position: fixed;
    top: 0;
    width: 100%;
}
.modal__bg{
    background: rgba(0,0,0,0.8);
    height: 100vh;
    position: absolute;
    width: 100%;
}
.modal__content{
    background: #fff;
    left: 50%;
    padding: 40px;
    position: absolute;
    top: 50%;
    transform: translate(-50%,-50%);
    width: 60%;
}

~~~

### js
~~~
$(function(){
    $('.js-modal-open').each(function(){
        $(this).on('click',function(){
            var target = $(this).data('target'); // modal0Xを取得
            var modal = document.getElementById(target); // modal0Xを持っているjs-modalを取得
            $(modal).fadeIn();
            return false;
        }); 
    });
    $('.js-modal-close').on('click',function(){
        $('.js-modal').fadeOut();
        return false;
    }); 
});


~~~
