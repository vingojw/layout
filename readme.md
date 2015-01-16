只是将常用的结构汇总。

虽然有了emmet 能够很方便的写html结构了。

但是感觉还是不快捷，
发现sublime text 能够自定义片段，那么我们可以自定义一些片段，然后按下tab，那么一个结构就ok了。

###例子

比如 nav  然后按tab键 ，那么一个nav结构就出来了

```
  <ul class="nav">
    <li><a href=""></a></li>
    <li><a href=""></a></li>
    <li><a href=""></a></li>
    <li><a href=""></a></li>
    <li><a href=""></a></li>
  </ul>
  
```
相当于 ul.nav>li*4>a。

---------------

再来一个tab切换的

```
 <!--tab-->
  <div class="tab">
    <ul class="tab-header">
      <li><a href="#tab1"></a></li>
      <li><a href="#tab2"></a></li>
      <li><a href="#tab3"></a></li>
    </ul>
    <div class="tab-content">
      <div class="tab-panel" id="tab1"></div>
      <div class="tab-panel" id="tab2"></div>
      <div class="tab-panel" id="tab3"></div>
    </div>
  </div>
  
```

------------
slider，幻灯片切换的

```
 <!--slider-->
  <div class="slidershow">
    <div class="slider">
      <ul class="slider-item">
        <li>
          <a href=""><img src="" alt=""></a>
          <div class="sldier-caption">  <!--针对图片的描述-->
            <h4 class="title"></h4>
            <div class="caption-des"></div>
          </div>
        </li>
        <li>
          <a href=""><img src="" alt=""></a>
          <div class="sldier-caption">  <!--针对图片的描述-->
            <h4 class="title"></h4>
            <div class="caption-des"></div>
          </div>
        </li>
        <li>
          <a href=""><img src="" alt=""></a>
          <div class="sldier-caption">  <!--针对图片的描述-->
            <h4 class="title"></h4>
            <div class="caption-des"></div>
          </div>
        </li>
        <li>
          <a href=""><img src="" alt=""></a>
          <div class="sldier-caption">  <!--针对图片的描述-->
            <h4 class="title"></h4>
            <div class="caption-des"></div>
          </div>
        </li>
        <li>
          <a href=""><img src="" alt=""></a>
          <div class="sldier-caption">  <!--针对图片的描述-->
            <h4 class="title"></h4>
            <div class="caption-des"></div>
          </div>
        </li>
      </ul>
      <ol class="slider-control">  <!--页面index-->
        <li>1</li>
        <li>2</li>
        <li>3</li>
        <li>4</li>
        <li>5</li>
      </ol>
      <a href="" id="pre"></a>   <!--翻页-->
      <a href="" id="next"></a>
    </div>
  </div>

```

类似这样，我觉得可以提高效率。
这样当结构确定好之后，再具体情况具体分析，可能会轻松点，同一类布局最好只用写一遍。
那到底一共有多少种布局呢？，难道每种布局都要来一遍？我也不知道，慢慢摸索吧。

参考：[css解决方案--W3CPLUS](http://www.w3cplus.com/solution/index/index.html)




