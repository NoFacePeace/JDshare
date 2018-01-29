# 搭建京东首页(简版)

> 前端工程师的基本技能 - 写页面
[ppt](http://blog.orzcn.cn/JDshare/)

## HTML 和 CSS

1. 页面的结构设计
1. 页面的表现设计

## 步骤

1. 划分版块
1. 搭建骨架
1. 样式设计

## 实战环节

进入京东首页

[点击这里](https://www.jd.com)

### 划分版块

1. header

    ![header](/images/header.png)

1. banner

    ![banner](/images/banner.png)

1. content

    ![content](/images/content.png)

1. footer

    ![footer](/images/footer.png)

1. 代码

    ```html
    <html lang="en">
        <head>
            <meta charset="UTF-8">
            <title>JD</title>
        </head>
        <!-- 第一层结构 -->
        <body>
            <div id="header"></div>
            <div id="banner"></div>
            <div id="content"></div>
            <div id="footer"></div>
        </body>
    ```

    [效果图](demo/demo6.html)

### 搭建骨架

#### header

![header](/images/header.png)

```html
<!-- 第二层结构 -->
<div id="header">
    <div id="login"></div>
    <div id="logo"></div>
    <div id="search"></div>
    <div id="cart"></div>
    <div id="nav"></div>
</div>
```

#### login

![login](/images/login.png)

```html
<!-- 第三层结构 -->
<div id="login">
    <ul id="location">
        <li>北京</li>
    </ul>
    <ul id="message">
        <li>我的订单</li>
        <li>我的京东</li>
        <li>京东会员</li>
        <li>企业采购</li>
        <li>客户服务</li>
        <li>网站导航</li>
        <li>手机京东</li>
    </ul>
</div>
```

### 样式设计

[无样式页面](demo1.html)

#### 重置标签

```CSS
* {
    margin: 0px;
    padding: 0px;
}
ul {
    list-style: none;
}
```

[重置页面](demo2.html)

#### 块状元素浮动

```CSS
#location {
    float: left;
}
#message {
    float: right;
}
#message li{
    float: left;
}
```

[浮动](demo3.html)

#### 颜色

```CSS
#login {
    height: 40px;
    background-color: #e3e4e5;
    color: #999;
}
```
[颜色](demo4.html)

#### 边距

```CSS
#location {
    margin-left: 20%;
}
#message {
    margin-right: 4%;
}
ul li {
    margin-right: 10px;
}
```

[边距](demo5.html)

#### demo

[京东首页](demo.html)

## 总结 : 树 + 嵌套

![](/images/tree.png)

## 页面的价值

1. 提高页面对搜索引擎的亲和度
1. 代码高度压缩
1. 提升页面加载速度
1. 提升网页的整体价值
1. 优化页面至极致