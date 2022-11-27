css笔记 2022 11 13-2022 11 20
##CSS声明
CSS声明总是以分号结束，声明总以大括号括起来
```css
p {color:red;text-align:center;}
```
为了增强可读性，你可以每行只描述一个属性
```css
p
{
    color:red;
    text-align:center;
}
```
##CSS注释
css注释是以\/*开始，以\*/结束
```css
/*这是个注释*/
p
{
    text-align:center;
    /*这是另一个注释*/
    color:black;
    font-family:arial;
}
```
##CCSid&Class选择器
如果你要在HTML元素中设置CSS样式，你需要在元素中设置"id" 和 "class"选择器。
###id选择器
id 选择器可以为标有特定 id 的 HTML 元素指定特定的样式。

HTML元素以id属性来设置id选择器,CSS 中 id 选择器以 "#" 来定义。
例如：
```css
#para1
{
    text-align:center;
    color:red;
}
/*应用于元素属性para1*/
```
###Class选择器
class 选择器用于描述一组元素的样式，class 选择器有别于id选择器，class可以在多个元素中使用。

class 选择器在 HTML 中以 class 属性表示, 在 CSS 中，类选择器以一个点 . 号显示：
```CSS
.center {text-align:center;}
/*代表拥有center 类的 HTML 元素均为居中。*/
```
也可以指定特定的 HTML 元素使用 class。
```css
p.center {text-align:center;}
```
多个 class 选择器可以使用空格分开：
```css
.center { text-align:center; }
.color { color:#ff0000; }
```
##CSS样式表
当读到一个样式表时，浏览器会根据它来格式化 HTML 文档。
###外部样式表
当样式需要应用于很多页面时，外部样式表将是理想的选择。在使用外部样式表的情况下，你可以通过改变一个文件来改变整个站点的外观。每个页面使用 \<link> 标签链接到样式表。 \<link> 标签在（文档的）头部：
```css
<head>
<link rel="stylesheet" type="text/css" href="mystyle.css">
</head>
```
浏览器会从文件 mystyle.css 中读到样式声明，并根据它来格式文档。
###内部样式表
当单个文档需要特殊的样式时，就应该使用内部样式表。你可以使用 \<style> 标签在文档头部定义内部样式表
```css
<head>
<style>
hr {color:sienna;}
p {margin-left:20px;}
body {background-image:url("images/back40.gif");}
</style>
</head>
```
###内联样式
由于要将表现和内容混杂在一起，内联样式会损失掉样式表的许多优势。请慎用这种方法，例如当样式仅需要在一个元素上应用一次时。

要使用内联样式，你需要在相关的标签内使用样式（style）属性。Style 属性可以包含任何 CSS 属性。
```css
<p style="color:sienna;margin-left:20px">这是一个段落。</p>
/*改变了段落的颜色和左外边距*/
```
##CSS背景
CSS 背景属性用于定义HTML元素的背景。
###背景颜色
background-color 属性定义了元素的背景颜色.
```css
body {background-color:#b0c4de;}
```
CSS中，颜色值通常以以下方式定义:
* 十六进制 如"#ff0000"
* RGB 如"rgb(255,0,0)"
* 颜色名称  如："red"
###背景图像
background-image 属性描述了元素的背景图像.
默认情况下，背景图像进行平铺重复显示，以覆盖整个元素实体.
```css
body {background-image:url('paper.gif');}
```
####水平或垂直平铺
默认情况下 background-image 属性会在页面的水平或者垂直方向平铺。
```css
body
{
background-image:url('gradient2.png');
}
```
水平方向平铺
```css
body
{
background-image:url('gradient2.png');
background-repeat:repeat-x;
}
```
####设置定位与不平铺
设置不平铺
```css
body
{
background-image:url('img_tree.png');
background-repeat:no-repeat;
}
```
可以利用 background-position 属性改变图像在背景中的位置
```css
body
{
background-image:url('img_tree.png');
background-repeat:no-repeat;
background-position:right top;
}
```
