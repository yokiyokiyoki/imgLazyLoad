# 图片懒加载

- [预览](https://yokiyokiyoki.github.io/imgLazyLoad/.)

> 原理是非首屏的图片先赋予一个默认的图片地址，直到图片出现在视窗之内，才给它加载正确的资源

## 三种高度

- 图片距离顶部高度：el.offsetTop
- 视窗高度：window.innerHeight
- 滚动条滚动的高度：
  - 如果是以 html 为根元素，即写了 DTD,则是 document.documentElement.scrollTop；
  - 如果没写则是 document.body.scrollTop,是以 body 为根元素
