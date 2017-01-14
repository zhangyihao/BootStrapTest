# Grid System（栅格系统）
## Containers（容器）
Bootstrap 需要为页面内容和栅格系统(Grid System)包裹一个 **.container** 容器。我们提供了两个作此用处的类。
`.container`用于固定宽度并支持响应式布局
```html
<div class="container">
	.......
</div>
```
`.container-fluid`用于100%宽度，占据全部viewport的容器。
```html
<div class="container-fluid">
	.......
</div>
```
***注意，由于 padding 等属性的原因，这两种容器类不能互相嵌套。***


## Grid System（栅格系统）
Bootstrap 提供了一套响应式、移动设备优先的流式栅格系统，随着屏幕或视口（viewport）尺寸的增加，系统会自动分为最多12列。它包含了易于使用的预定义类，还有强大的mixin 用于生成更具语义的布局。


####简介
栅格系统使用一系列的行和列的组合来进行界面的布局，下面是栅格系统的工作原理：

- Rows（行）必须包含在容器`.container`（固定宽度）或者`.container-fluid`（100%宽度）中才能正确排列布局。
- 通过Row（行）在水平方向上创建一组列。
- 所有内容应该放置在列（Columns）中，而且只有列（Columns）才可以是行（Row）的子元素。
- 使用预定义的类，例如`.row`和`.col-xs-4`可以快速的创建格栅布局。
- 通过为“列（column）”设置 padding 属性，从而创建列与列之间的间隔（gutter）。通过为 .row 元素设置负值 margin 从而抵消掉为 .container 元素设置的 padding，也就间接为“行（row）”所包含的“列（column）”抵消掉了padding。
- 如果在一行中超过了12列，多余的列将会作为一个新的整体另起一行排列。

示例代码：
```html
<div class="container-fluid">
	<div class="row">
	  <div class="col-md-8">.col-md-8</div>
	  <div class="col-md-4">.col-md-4</div>
	</div>
	<div class="row">
	  <div class="col-md-4">.col-md-4</div>
	  <div class="col-md-4">.col-md-4</div>
	  <div class="col-md-4">.col-md-4</div>
	</div>
	<div class="row">
	  <div class="col-md-6">.col-md-6</div>
	  <div class="col-md-6">.col-md-6</div>
	</div>
</div>

```
效果：
![栅格系统示例1](http://i.imgur.com/18F5d46.png)