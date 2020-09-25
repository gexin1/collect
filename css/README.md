#### 多行省略号
```html
<style type="text/css">
	.wrap {
    height: 40px;
    line-height: 20px;
    overflow: hidden;
}

.wrap .text {
    float: right;
    margin-left: -5px;
    width: 100%;
    word-break: break-all;
}

.wrap::before {
    float: left;
    width: 5px;
    content: '';
    height: 40px;
}

.wrap::after {
    float: right;
    text-align: right;
    content: "...";
    height: 20px;
    line-height: 20px;
    /* 为三个省略号的宽度 */
    width: 3em;
    /* 使盒子不占位置 */
    margin-left: -3em;
    /* 移动省略号位置 */
    position: relative;
    left: 100%;
    top: -20px;
    padding-right: 5px;
    /* 显示更好的效果 */
    background: -webkit-gradient(linear, left top, right top, from(rgba(255, 255, 255, 0)), to(white), color-stop(50%, white));
    background: -moz-linear-gradient(to right, rgba(255, 255, 255, 0), white 50%, white);
    background: -o-linear-gradient(to right, rgba(255, 255, 255, 0), white 50%, white);
    background: -ms-linear-gradient(to right, rgba(255, 255, 255, 0), white 50%, white);
    background: linear-gradient(to right, rgba(255, 255, 255, 0), white 50%, white);
}

</style>
<div class="wrap">
  <div class="text">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Dignissimos labore sit vel itaque delectus atque quos magnam assumenda quod architecto perspiciatis animi.</div>
</div>
```


