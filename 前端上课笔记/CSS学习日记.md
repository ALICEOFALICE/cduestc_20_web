# CSS学习日记

CSS分链接式和内联式，推荐链接式。

如果希望网页美观、大方、并且升级轻松、维护方便、就需要css，实现结构与表现分离

CSS可以提供很多属性：

|    标签    |        值        |     意义     |
| :--------: | :--------------: | :----------: |
|    font    |      字体名      | 修改字体属性 |
|   color    |     RGB色值      | 修改字体颜色 |
| background | 文件位置/RGB色域 | 修改背景属性 |
|   float    |     浮动属性     |   浮动属性   |

同时CSS非常灵活，既可以插入HTML，也可单独设立一个文件，如果为独立文件，则必须要以css结尾

## CSS样式规则选择器

CSS语法规则为：选择器(属性1,属性值1;属性2,属性值2)

CSS分为三种插入方式

	- 行内式
	- 内嵌式
	- 链入式

具体看下面的分标签

## 行内式

用得少，基本没啥用，把style插入标签就行

```html
<div style="color: #0000FF; font-size:30px">
    这是行内式
</div>
```



## 内嵌式

内链接式采用`style`参数，需要插入`head`标签之中

PS：内联式不需要额外创建文件，如果需要高度整合可以用联式

```html
<head>
    <style type="text/css">
        p{
            color="green"
        }
    </style>
</head>
```

## 链入式

外链式需要先使用`link`标签导入，具体如下

```html
<!-- 这是HTML文档内的东西 -->
<head>
    <link rel="stylesheet" type="text/css" href="css文件位置">
</head>
```

导入后需要在css文件内修改，具体如下

```css
<!-- 这是css文件内的东西 -->
#id1{
	color:red;
	font-size:30px;
}
<!--↑这是ID选择器-->
.class1{
	color:green;
	font-size:40px
}
<!--↑这是class选择器-->
p{
	color:blue;
	font-size;
}
<!--↑这是标签选择器-->
```

## 选择器

选择器分为三种

- 标签选择器
- 类选择器
- ID选择器

三种区别不大，标签选择器范围最大（慎重使用）,具体可以看下面

```css
<!-- 这是css文件内的东西 -->
#id1{
	color:red;
	font-size:30px;
}
<!--↑这是ID选择器-->
.class1{
	color:green;
	font-size:40px
}
<!--↑这是class（类）选择器-->
p{
	color:blue;
	font-size;
}
<!--↑这是标签选择器-->
```

更多看选择器专题