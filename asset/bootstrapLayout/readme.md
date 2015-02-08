#bootstrap3  关于栅格的片段

bootstrap中默认的是15px间距，然后最宽是1170px

如果有一个是 宽度1180间距是20呢？
因为修改了间距，那么就要变成 1200 然后修改左右间距10px，这样就是1180了

```
.col-xs-12 {
  width: 100%;
}

.col-xs-11 {
  width: 91.66666667%;  11/12  0.916666667
}

.col-xs-10 {
  width: 83.33333333%;  10/12  0.833333333
}

.col-xs-9 {
  width: 75%;          9/12   0.75
}
```

因为是12栅格，所以这里的比例就是除以12得来的。

##col-xs col-sm col-md col-lg 关系

超小屏幕 手机 (<768px)              .col-xs-

小屏幕 平板 (≥768px)                  .col-sm-

中等屏幕 桌面显示器 (≥992px)    .col-md-

大屏幕 大桌面显示器 (≥1200px)  .col-lg-

bootstrap 你可以给一个div设置

class="col-sm-3 col-md-6 col-lg-12"

代表 在小屏幕上按照3列展示,中等屏幕6列展示，大屏幕满格展示。

##自定义宽度间距

bootstrap中默认的是15px间距，然后最宽是1170px。

如果有一个是 宽度1180间距是20呢？

通过如下修改

```
@media (min-width: 1200px) {
  .container {
    width: 1200px;  这里就要变成 1200 然后修改左右间距10px，这样就是1180了
  }
}
...
...
.container {
  padding-right: 10px; 修改左右间距10px
  padding-left: 10px; 修改左右间距10px
  margin-right: auto;
  margin-left: auto;
}
.container-fluid {
  padding-right: 10px; 修改左右间距10px
  padding-left: 10px; 修改左右间距10px
  margin-right: auto;
  margin-left: auto;
}
.row {
  margin-right: -10px; 修改左右间距10px
  margin-left: -10px; 修改左右间距10px
}
.col-xs-1, .col-sm-1, .col-md-1, .col-lg-1, .col-xs-2, .col-sm-2, .col-md-2, .col-lg-2, .col-xs-3, .col-sm-3, .col-md-3, .col-lg-3, .col-xs-4, .col-sm-4, .col-md-4, .col-lg-4, .col-xs-5, .col-sm-5, .col-md-5, .col-lg-5, .col-xs-6, .col-sm-6, .col-md-6, .col-lg-6, .col-xs-7, .col-sm-7, .col-md-7, .col-lg-7, .col-xs-8, .col-sm-8, .col-md-8, .col-lg-8, .col-xs-9, .col-sm-9, .col-md-9, .col-lg-9, .col-xs-10, .col-sm-10, .col-md-10, .col-lg-10, .col-xs-11, .col-sm-11, .col-md-11, .col-lg-11, .col-xs-12, .col-sm-12, .col-md-12, .col-lg-12 {
  position: relative;
  min-height: 1px;
  padding-right: 10px; 修改左右间距10px
  padding-left: 10px; 修改左右间距10px
}
```

布局的关键是以下这段代码

```
* {
-webkit-box-sizing: border-box;
-moz-box-sizing: border-box;
box-sizing: border-box;
}
```
