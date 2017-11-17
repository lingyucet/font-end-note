# font-end-note

1、jq.lazyload 使用：<br> 
图片加载不全的问题 <br>
首先：必须设置图片display：none <br>
触发事件：<br>

<body>
<script>  

$('img.lazy').lazyload({
        event : "sporty",
        placeholder:''
    });

    var timeout = setTimeout(function() { //ie必须先加载图片
        $("img.lazy").trigger("sporty");
    },100);
    
</srcript>
</doby>
