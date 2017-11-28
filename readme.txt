 基于 https://cdn.bootcss.com/jquery/3.2.1/jquery.min.js 下写的一个轮播图插件
 使用需要引入jquery库，如果不兼容使用以上版本jquery

   type 为轮播样式提供两个参数
   "fade" 淡入淡出
   "LRslide" 滑动
 
 示例
 <div id="banner">
    <div class="pic">
        <ul>
            <li><a href=""><img src="img/1.jpg" alt=""></a></li>
            <li><a href=""><img src="img/2.jpg" alt=""></a></li>
            <li><a href=""><img src="img/3.jpg" alt=""></a></li>
            <li><a href=""><img src="img/4.jpg" alt=""></a></li>
            <li><a href=""><img src="img/5.jpg" alt=""></a></li>
        </ul>
    </div>

    <div class="tab">
        <ul>
            <li></li>
            <li></li>
            <li></li>
            <li></li>
            <li></li>
        </ul>
    </div>
    <div class="btn">
        <div class="left"> </div>
        <div class="right"> </div>
    </div>

 $("#banner").banner({
        type : "LRslide",	 // type 为轮播样式提供两个参数"fade" 淡入淡出  ,"LRslide" 滑动,不传此参数默认为“fade”
        picE : ".pic ul li", //图片
        tabE : ".tab ul li", //导航选项卡
        btnE : ".btn div",	 //导航按钮
        time : 2000			 //自动播放间隔毫秒值,不给不自动
    });
  