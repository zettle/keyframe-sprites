# 多个图片合并成雪碧图

参考资料: http://wanlimm.com/77201809146901.html

```css
.box {
    width: {{imgWidth}}px;
    height: {{imgHeight}}px;
    background: url('./sprite.png') no-repeat;
    animation: run {{duration}}s steps({{imgList.length}}, end) infinite;
}
@keyframes run {
    0% { background-position: 0 0; }
    100% { background-position: -{{canvasWidth}}px 0; }
}
```

