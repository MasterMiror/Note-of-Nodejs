#html笔记

多来源于菜鸟教程，跟着写。联系在html_file文件中。

p标签作为段落标签

h标签作为头部标签,h后的序号代表标签级别,数目约小级别越高.h1-h6

head标签作为标题标签

body标签作文件主体

a标签用以指示超链接 href用以指示链接地址 文本用以表示链接名称

mg标签用于表示图像 src指示资源路径 width height指示图片尺寸

br标签是换行符

*HTML对大小写不敏感*

html 大部分标签都带有属性 分别定义标签的各类参数 常见的诸如 字体、字号、图的宽度、高度等等.参见链接https://www.runoob.com/tags/html-reference.html.

\<hr>标签用于分割内容 这东西就是一条水平线

\<br>是换行标签

\<b>加粗 \<i>斜体 \<strong> \<em>
突出

\<sub>下标 \<sup>上标

\<ins>定义插入字

\<del>定义删除字

\<code>定义代码标签

\<kbd>键盘定义码

\<samp>定义计算机代码样本

\<var>定义变量

\<pre>定义预格式文本

\<a href="https://www.runoob.com/" target="_blank" rel="noopener noreferrer">访问菜鸟教程!</a>

target和rel标记超链接.

id属性是在文档中插入ID.

\<head> \<base> \<link> \<style> \<meta> \<script>标签顾名思义 除\<head>以外标签都包含在\<head>标签中

---

#CSS概述

CSS Cascading Style Sheets 层叠式样式表

定义如何现实html元素,样式通常存储在样式表中.外部样式通常存储在CSS文件中.

css范例

```html

<!DOCTYPE html>
<html>
<head>
<meta charset="utf-8">
<title>菜鸟教程(runoob.com)</title>
<style>
p
{
	color:red;
	text-align:center;
}
</style>
</head>

<body>
<p>Hello World!</p>
<p>这个段落采用CSS样式化。</p>
</body>
</html>

```

其中

```html
p
{
	color:red;
	text-align:center;
}
```


的部分定义了对\<p>标签的渲染


id选择器可以标记有特定id的html元素指定特定的定义样式.css中id选择器使用\#符号来表示.

class选择器用于描述一组元素的样式,class有别于id选择器,class可以在多个元素中使用.

ps:类的第一个名字不能使用数字,否则无法在mozilla和Firefox中起作用.

```html
<!DOCTYPE html>
<html>
<head>
<meta charset="utf-8">
<title>菜鸟教程(runoob.com)</title>
<style>
.center
{
	text-align:center;
}
</style>
</head>

<body>
<h1 class="center">标题居中</h1>
<p class="center">段落居中。</p>
</body>
</html>
```


```html
<!DOCTYPE html>
<html>
<head>
<meta charset="utf-8">
<title>菜鸟教程(runoob.com)</title>
<style>
p.center
{
	text-align:center;
}
</style>
</head>

<body>
<h1 class="center">这个标题不受影响</h1>
<p class="center">这个段落居中对齐。</p>
</body>
</html>
```

插入css样式表的方法有三种:

1.外部样式表

2.内部样式表

3.内联样式
