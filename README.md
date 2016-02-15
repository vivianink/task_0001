## task_0001

## Index Page

###笔记

######1. 页面实际内容宽度为980px，头部背景、大图、底部背景均为100%宽，当浏览器宽度低于980px时，页面宽度不变，允许出现横向滚动条。右上角的Github图标在浏览器低于980px时消失。
实现如下：

```css
@media (max-width: 980px) {
    html,
    body {
        width: 980px;
        overflow: scroll;
    }
    .header_hd .github_icon {
        display: none;
    }
}
```

######2. 透明渐变背景的应用：

```css
 div {
    background: -webkit-linear-gradient(top, rgba(255, 255, 255, .7), rgba(255, 255, 255, .5), rgba(255, 255, 255, 0) 25%);
 }
```

参数说明：<br/>
- top: 为颜色开始的起点，例如 left top等；或者为颜色渐变的方向，例如 to right；此外还可设置为渐变方向角度，例如 45deg。
     不设置起点或方向则会形成一个同心圆。
- 颜色值： 可跟多个颜色，且可规定颜色的长度，例如 rgba(255, 255, 255, 0) 25% 

参考资料：
- <a href="http://www.w3schools.com/css/css3_gradients.asp" target="_blank">CSS3 Gradients</a>
- <a href="http://www.75team.com/archives/174" target="_blank">跨浏览器背景色渐变和透明</a>

###余留问题：

######1. IE中实现渐变透明背景

## Blog page

###问题：
- 1.display:inline-block空隙问题，搜索栏的另外样式方法
- 2.两栏布局常见方式
- 3.为啥当侧栏搜索块内两个子元素改为float后，其父框即.aside_search被撑得很高？
为啥为父元素设置 overflow:hidden后就没事儿了？

## gallery page

######1.div中的img标签和div产生间隙，设置img:display:block可解决。



