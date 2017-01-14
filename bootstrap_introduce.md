# Bootstrap介绍
Bootstrap是基于HTML5和CSS3开发的一款响应式web框架。
Bootstrap提供了丰富的web组件，包括：下拉菜单、按钮、导航、导航条、分页、缩略图、进度条等等。同时内置了12个JQuery插件，包括：模式对话框、标签页、弹出框等。

当前版本：v3.3.7
官网地址：[getbootstrap.com](http://getbootstrap.com)
中文网站地址：[v3.bootcss.com](http://v3.bootcss.com/)

## 基本模版
bootstrap标准模版，可根据需要进行调整。
``` html
<!DOCTYPE html>
<html lang="zh-CN">
  <head>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <!-- The above 3 meta tags *must* come first in the head; any other head content must come *after* these tags -->
    <title>Bootstrap 101 Template</title>

    <!-- Bootstrap -->
    <link href="css/bootstrap.min.css" rel="stylesheet">

    <!-- HTML5 shim and Respond.js for IE8 support of HTML5 elements and media queries -->
    <!-- WARNING: Respond.js doesn't work if you view the page via file:// -->
    <!--[if lt IE 9]>
      <script src="https://oss.maxcdn.com/html5shiv/3.7.3/html5shiv.min.js"></script>
      <script src="https://oss.maxcdn.com/respond/1.4.2/respond.min.js"></script>
    <![endif]-->
  </head>
  <body>
    <h1>Hello, world!</h1>

    <!-- jQuery (necessary for Bootstrap's JavaScript plugins) -->
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/1.12.4/jquery.min.js"></script>
    <!-- Include all compiled plugins (below), or include individual files as needed -->
    <script src="js/bootstrap.min.js"></script>
  </body>
</html>
```
**说明：**
1. script脚本的引入放在`body`标签的最后边.
2. 由于bootstrap的js脚本依赖jquery，所以要先引入jquery.min.js。
3. 依赖的jquery的最低版本为1.9.1。
## 浏览器和设备支持情况

### 被支持的浏览器
 --|Chrome|Firefox|Safari|Internet Explorer|Opera
 --|------|-------|------|-----|-
 Android|支持|支持|不支持|不支持|不支持
 IOS|支持|支持|支持|不支持|不支持
 Mac|支持|支持|支持|不支持|支持
 windows|支持|支持|不支持|支持|支持

 _**注意： IE只支持IE8-11**_
 Internet Explorer 8 需要 [Respond.js](https://github.com/scottjehl/Respond/blob/master/README.md#cdnx-domain-setup) 配合才能实现对媒体查询（media query）的支持。

### IE兼容模式

Bootstrap 不支持 IE 古老的兼容模式。为了让 IE 浏览器运行最新的渲染模式下，建议将此 `<meta>` 标签加入到你的页面中：
```html
 <meta http-equiv="X-UA-Compatible" content="IE=edge">
```
### 国产浏览器高速模式

国内浏览器厂商一般都支持兼容模式（即 IE 内核）和高速模式（即 webkit 内核），不幸的是，所有国产浏览器都是默认使用兼容模式，这就造成由于低版本 IE （IE8 及以下）内核让基于 Bootstrap 构建的网站展现效果很糟糕的情况。
将下面的 <meta> 标签加入到页面中，可以让部分国产浏览器默认采用高速模式渲染页面：
```html
<meta name="renderer" content="webkit">
```