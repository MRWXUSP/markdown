html笔记 2022 11 13-2022 11 20

#基础

##HTML标题
>HTML标题

同markdown,html标题也分级，共为六级[^0]
[^0]:浏览器会自动地在标题后换行
>\<h1>一级标题\</h1>
>\<h2>二级标题\</h2>
>.......

>HTML水平线

\<hr>可以创建水平线
```html
<p>这是一个段落。</p>
<hr>
<p>这是一个段落。</p>
<hr>
<p>这是一个段落。</p>
```
>HTML注释

HTML也有注释，浏览器不会显示注释，但可以提高代码可读性
```html
<!-- 这是一个注释 -->
```

##HTML段落
HTML的段落是通过标签\<p>来定义的
```html
<p>这是一个段落</p>
```
>HTML折行

```html
<p>这个<br>段落<br>演示了分行的效果</p>
```
<br /> 元素是一个空的 HTML 元素。由于关闭标签没有任何意义，因此它没有结束标签。

##HTML链接
HTML 链接是通过标签 \<a> 来定义的
>\<a href="www.bilibili.com">这是一个链接\</a>

它的格式很简单
\<a href="url">链接文本\</a>
###链接属性
>target属性

使用 target 属性，你可以定义被链接的文档在何处显示。
```html
<a href="https://www.runoob.com/" target="_blank" rel="noopener noreferrer">访问菜鸟教程!</a>
<!--这个链接将会在新窗口打开-->
```
>id属性

id 属性可用于创建一个 HTML 文档书签。
书签不会以任何特殊方式显示，即在 HTML 页面中是不显示的，所以对于读者来说是隐藏的。
```html
<a id="tips">有用的提示部分</a>
```


##HTML图像

HTML图像是通过标签 \<img> 来定义的
>\<img decoding="async" src="/images/logo.png" width="258" height="39" \/>

#元素
HTML元素分为：开始标签 元素内容 结束标签
注:HTML元素没有内容时被叫做空元素

#属性
* HTML元素可以设置属性
* 属性可以添加附加信息
* 属性以名称/值对的形式出现

例如下面的链接
```html
<a href="http://www.runoob.com">这是一个链接</a>>
```
此属性就为herf[^1]，双引号内被称为属性值
[^1]:属性与属性值对大小写不敏感，但尽量小写

##HTML文字格式
>标签

HTML使用标签\<b>("blod")加粗与\<i>("italic")斜体等对输出的文本进行格式化