# 文字渐变效果和镂空效果

[预览效果](https://htmlpreview.github.io/?https://github.com/Xudake/text-fill-color/blob/master/index.html)
## 主要使用的属性
+ background: linear-gradient(125deg,#fff,#000)
+ text-fill-text
+ text-stroke
+ background-clip

## 三种效果
>文字渐变
```
.text1 {
    margin: 0 auto;
    font-size: 60px;
    text-align: center;
    font-weight: bold;
    /* 背景颜色渐变 */
    background: linear-gradient(125deg,red,#6a38ec);

    /* 背景区域设成文字 */
    -webkit-background-clip: text;
    /* color: transparent; */

    /* 文字填充设置成透明 */
    -webkit-text-fill-color: transparent;
}
```
>文字描边
```
.text2 {
    margin: 0 auto;
    font-size: 60px;
    text-align: center;
    font-weight: bold;
    
    /* 文字填充成透明 */
    -webkit-text-fill-color:transparent;

    /* 文字描边成红色 */
    -webkit-text-stroke:1px red; 
}
```


>文字图片背景
```
.text3 {
    margin: 0 auto;
    font-size: 60px;
    line-height: 1;
    text-align: center;
    font-weight: bold;

    /* 文字背景设置成一张图片 */
    background: url(http://placekitten.com/500/500) repeat center center;
    background-size: contain;

    /* 背景区域设成文字 */
    -webkit-background-clip: text;

    /* 文字填充：透明 */
    -webkit-text-fill-color: transparent;
}
```
---
### tips: 猫咪占位符

[猫咪: http://placekitten.com/500/500](http://placekitten.com/500/500)

设置不同的数值~ 先显示不同大小和样子的猫咪图片

