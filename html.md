## HTML

html是超文本标记语言，是一种用于创建网页的标准标记语言。

一个html页面会包含几个基本要素

```html
<!-- 声明为html5文档 -->
<!DOCTYPE html>
<html>
    <!-- 头部元素 -->
    <head>
         <!-- 定义网页编码格式为 utf-8 -->
        <meta charset="utf-8">
        <!-- 网页的标题 -->
        <title>HTML</title>
    </head>
    <!-- 网页内容的可见元素 -->
    <body>
       我是一个网页
    </body>
</html>
```

HTML 标记标签通常被称为 HTML 标签 (HTML tag)。

- HTML 标签是由尖括号**<>**包围的关键词，比如 <html>

- HTML 标签通常是成对出现的，比如 <body> 和 </body>

- 标签对中的第一个标签是开始标签，第二个标签是结束标签

- 开始和结束标签也被称为开放标签和闭合标签

    

## HTML head 元素

head 元素包含了所有的头部标签元素。在 <head>元素中你可以插入脚本（scripts）, 样式文件（CSS），及各种meta信息。

可以添加在头部区域的元素标签为: <title>, <style>, <meta>, <link>, <script> 

### 1.title

title 标签定义了当前文档的标题。

**title在 HTML文档中是必须的**

title元素:

- 定义了浏览器工具栏的标题
- 当网页添加到收藏夹时，显示在收藏夹中的标题
- 显示在搜索引擎结果页面的标题

### 2.link

<link> 标签定义了文档与外部资源之间的关系。

<link> 标签通常用于链接到样式表:

```html
<head>
    <link rel="stylesheet" type="text/css" href="mystyle.css">
</head>
```

### 3.style

style标签定义了HTML文档的样式


在<style> 元素中你也可以直接添加样式来渲染 HTML 文档:

```html
<head>
<style type="text/css">
	body {
        background-color:yellow
    }
	p {
        color:blue
    }
</style>
</head>
```

### 4.meta

meta标签描述了一些基本的元数据。

meta 标签提供了元数据.元数据也不显示在页面上，但会被浏览器解析。

META 元素通常用于指定网页的**描述**，**关键词**，文件的最后修改时间，作者，和其他元数据。

元数据可以使用于浏览器（如何显示内容或重新加载页面），搜索引擎（关键词），或其他Web服务。

meta 一般放置于 <head> 区域

为搜索引擎定义关键词:

```
<meta name="keywords" content="朝夕教育，在线教育">
```

为网页定义描述内容:

```
<meta name="description" content="编程 教程">
```

定义网页作者:

```
<meta name="author" content="Tina">
```

每30秒钟刷新当前页面:

```
<meta http-equiv="refresh" content="30">
```

### 5.script

script标签用于加载脚本文件

## HTML head 元素

| 标签     | 描述                               |
| :------- | :--------------------------------- |
| <head>   | 定义了文档的信息                   |
| <title>  | 定义了文档的标题                   |
| <link>   | 定义了一个文档和外部资源之间的关系 |
| <meta>   | 定义了HTML文档中的元数据           |
| <script> | 定义了客户端的脚本文件             |
| <style>  | 定义了HTML文档的样式文件           |



## HTML 元素

HTML 文档由 HTML 元素定义。

元素就是标签

## HTML 元素语法

- HTML 元素以**开始标签**起始
- HTML 元素以**结束标签**终止
- **元素的内容**是开始标签与结束标签之间的内容
- 某些 HTML 元素具有**空内容**
- 空元素**在开始标签中进行关闭**（以开始标签的结束而结束）
- 大多数 HTML 元素可拥有**属性**
- 元素和元素之间可以是嵌套关系
- **标签都是小写**



##   属性

​	属性是 HTML 元素提供的附加信息

- HTML 元素可以设置**属性**

- 属性可以在元素中添加**附加信息**

- 属性一般描述于**开始标签**

- 属性总是以名称/值对的形式出现，**比如：name="value"**。

- 属性值应该始终被包括在引号内。

- 属性和属性值对大小写不敏感（但是推荐使用小写）

    

    下面列出了适用于大多数 HTML 元素的属性：

    | 属性  | 描述                                                         |
    | :---- | :----------------------------------------------------------- |
    | class | 为html元素定义一个或多个类名（classname）(类名从样式文件引入) |
    | id    | 定义元素的唯一id                                             |
    | style | 规定元素的行内样式（inline style）                           |
    | title | 描述了元素的额外信息 (作为工具条使用)                        |

    

## HTML标签

### 1.标题

​		标题（Heading）是通过 <h1> - <h6> 标签进行定义的。

​         <h1> 定义最大的标题。 <h6> 定义最小的标题。

```html
<h1>这是一个标题。</h1>
<h2>这是一个标题。</h2>
<h3>这是一个标题。</h3>
<h4>这是一个标题。</h4>
<h5>这是一个标题。</h5>
<h6>这是一个标题。</h6>
```

请确保将 HTML 标题 标签只用于标题。不要仅仅是为了生成**粗体**或**大号**的文本而使用标题。

搜索引擎使用标题为您的网页的结构和内容编制索引。

因为用户可以通过标题来快速浏览您的网页，所以用标题来呈现文档结构是很重要的。

应该将 h1 用作主标题（最重要的），其后是 h2（次重要的），再其次是 h3，以此类推。



### 2.水平线

**<hr/>**标签 HTML 页面中创建水平线。

```html
<h1>这是一个标题。</h1>
<hr/>
<h2>这是一个标题。</h2>
```



### 3.注释

注释是用作提高其可读性，使代码更易被人理解。浏览器会忽略注释，也不会显示它们。

**注释:** 开始括号之后（左边的括号）需要紧跟一个叹号，结束括号之前（右边的括号）不需要，合理地使用注释可以对未来的代码编辑工作产生帮助。

```HTML
<!-- 这是一个标题 -->
<h1>这是一个标题。</h1>
```



### 4.段落

段落是通过 <p> 标签定义的，<p>标签是一个块级元素

```HTML
<p>这是一个段落 </p>
<p>这是另一个段落</p>
```



### 5.换行

**br**标签会在不产生一个新段落的情况下进行换行

**br**标签是一个空元素。由于关闭标签没有任何意义，因此它没有结束标签。

```HTML
<p>这个<br>段落<br>演示了分行的效果</p>
```



### 6.文本格式化

| 标签     | 描述         |
| :------- | :----------- |
| <b>      | 定义粗体文本 |
| <em>     | 定义着重文字 |
| <i>      | 定义斜体字   |
| <small>  | 定义小号字   |
| <strong> | 定义加重语气 |
| <sub>    | 定义下标字   |
| <sup>    | 定义上标字   |
| <ins>    | 定义插入字   |
| <del>    | 定义删除字   |

```

```

### 7.链接

​	HTML使用标签 <a>来设置超文本链接。

超链接可以是一个字，一个词，或者一组词，也可以是一幅图像，您可以点击这些内容来跳转到新的文档或者当前文档中的某个部分。

当您把鼠标指针移动到网页中的某个链接上时，箭头会变为一只小手。

在标签<a> 中使用了href属性来描述链接的地址。

默认情况下，链接将以以下形式出现在浏览器中：

- 一个未访问过的链接显示为蓝色字体并带有下划线。

- 访问过的链接显示为紫色并带有下划线。

- 点击链接时，链接显示为红色并带有下划线。

- target属性可以决定链接以什么形式打开

    ```HTML
    <a href="https://www.baidu.com/">百度</a>
    <a target="_blank" href="https://www.baidu.com/">百度</a>
    ```

### 8.图片

在 HTML 中，图像由<img> 标签定义。

<img> 是空标签，意思是说，它只包含属性，并且没有闭合标签。

要在页面上显示图像，你需要使用源属性（src）。src 指向图像的 URL 地址。

alt 属性用来为图像定义一串预备的可替换的文本。替换文本属性的值是用户定义的。

```HTML
<img src="https://www.zhaoxiedu.net/static/imgs/companyInfo/Logo2.png" alt="logo">
```

### 9.表格

#### 1.基础表格

表格由 <table> 标签来定义。每个表格均有若干行（由 <tr> 标签定义），每行被分割为若干单元格（由 <td> 标签定义）。字母 td 指表格数据（table data），即数据单元格的内容。数据单元格可以包含文本、图片、列表、段落、表单、水平线、表格等等。

```html
<table border="1">
    <tr>
        <td>row 1, cell 1</td>
        <td>row 1, cell 2</td>
    </tr>
    <tr>
        <td>row 2, cell 1</td>
        <td>row 2, cell 2</td>
    </tr>
</table>
```

#### 2.表头

表格的表头使用 <th> 标签进行定义。

浏览器会把表头显示为粗体居中的文本：

```html
<table border="1">
    <tr>
        <th>Header 1</th>
        <th>Header 2</th>
    </tr>
    <tr>
        <td>row 1, cell 1</td>
        <td>row 1, cell 2</td>
    </tr>
    <tr>
        <td>row 2, cell 1</td>
        <td>row 2, cell 2</td>
    </tr>
</table>
```

#### 3.合并单元格

合并单元格可以通过给**td**或者**th**设置**colspan**或者**rowspan**进行和**行合并**以及**列合并**

**colspan**：合并列

**rowspan**：合并行

```HTML
<h4>横跨两列的单元格：</h4>
<table border="1">
<tr>
  <th>姓名</th>
  <th colspan="2">电话</th>
</tr>
<tr>
  <td>Bill Gates</td>
  <td>555 77 854</td>
  <td>555 77 855</td>
</tr>
</table>

<h4>横跨两行的单元格：</h4>
<table border="1">
<tr>
  <th>姓名</th>
  <td>Bill Gates</td>
</tr>
<tr>
  <th rowspan="2">电话</th>
  <td>555 77 854</td>
</tr>
<tr>
  <td>555 77 855</td>
</tr>
</table>
```

#### 4.单元格距离

**cellpadding**：设置单元格内边距

**cellspacing**：设置单元格外边距

```HTML
<h4>cellpadding</h4>
<table border="1"
       cellpadding="10">
<tr>
  <td>First</td>
  <td>Row</td>
</tr>   
<tr>
  <td>Second</td>
  <td>Row</td>
</tr>
</table>

<h4> cellspacing</h4>
<table border="1" 
cellspacing="10">
<tr>
  <td>First</td>
  <td>Row</td>
</tr>   
<tr>
  <td>Second</td>
  <td>Row</td>
</tr>
</table>
```

#### 5.单元格内容排列方式

**align**：left | right

```html
<table width="400" border="1">
 <tr>
  <th align="left">消费项目....</th>
  <th align="right">一月</th>
  <th align="right">二月</th>
 </tr>
 <tr>
  <td align="left">衣服</td>
  <td align="right">$241.10</td>
  <td align="right">$50.20</td>
 </tr>
 <tr>
  <td align="left">化妆品</td>
  <td align="right">$30.00</td>
  <td align="right">$44.45</td>
 </tr>
 <tr>
  <td align="left">食物</td>
  <td align="right">$730.40</td>
  <td align="right">$650.00</td>
 </tr>
 <tr>
  <th align="left">总计</th>
  <th align="right">$1001.50</th>
  <th align="right">$744.65</th>
 </tr>
</table>

```

####  HTML 表格标签

| 标签    | 描述           |
| :------ | :------------- |
| <table> | 定义表格       |
| <th>    | 定义表格的表头 |
| <tr>    | 定义表格的行   |
| <td>    | 定义表格单元   |
| <thead> | 定义表格的页眉 |
| <tbody> | 定义表格的主体 |
| <tfoot> | 定义表格的页脚 |



### 10.列表

列表区分为有序列表和无需列表

#### 1.有序列表

有序列表是一列项目，列表项目使用数字进行标记。

有序列表始于 <ol> 标签。每个列表项始于 <li> 标签

可以通过**type**属性修改有序列表的样式
**type**: A| a| I | i

```HTML
<ol>
<li>内容1</li>
<li>内容2</li>
</ol>
```

#### 2.无序列表

无序列表也是一个项目的列表，此列项目使用粗体圆点（典型的小黑圆圈）进行标记。

无序列表始于 <ul> 标签。每个列表项始于 <li>

可以通过**type**属性修改无序列表的样式
**type**: disc | circle | square

```HTML
<ul>
<li>内容1</li>
<li>内容2</li>
</ul>
```

3.自定义列表

自定义列表不仅仅是一列项目，而是项目及其注释的组合。

自定义列表以 <dl> 标签开始。每个自定义列表项以 <dt> 开始。每个自定义列表项的定义以 <dd> 开始

```HTML
<dl>
<dt>Coffee</dt>
<dd>Black hot drink</dd>
<dt>Milk</dt>
<dd>White cold drink</dd>
</dl>
```

#### 列表标签

| 标签 | 描述               |
| :--- | :----------------- |
| <ol> | 定义有序列表。     |
| <ul> | 定义无序列表。     |
| <li> | 定义列表项。       |
| <dl> | 自定义定义列表。   |
| <dt> | 自定义定义项目。   |
| <dd> | 自定义定义的描述。 |



### 11.区块 div 和 span

HTML 可以通过 <div> 和 <span>将元素组合起来。

大多数 HTML 元素被定义为**块级元素**或**内联元素**。

块级元素在浏览器显示时，通常会以新行来开始（和结束）

实例: <h1>, <p>, <ul>, <table>

内联元素在显示时通常不会以新行开始

实例: <b>, <td>, <a>, <img>

####  1.div 元素

HTML <div> 元素是块级元素，它可用于组合其他 HTML 元素的容器。

<div> 元素没有特定的含义。除此之外，由于它属于块级元素，浏览器会在其前后显示折行。

如果与 CSS 一同使用，<div> 元素可用于对大的内容块设置样式属性。

div 元素的另一个常见的用途是文档布局

```HTML
<div>只是一个块级元素<div>
```

#### 2.span元素

TML <span> 元素是内联元素，可用作文本的容器

<span> 元素也没有特定的含义。

当与 CSS 一同使用时，<span> 元素可用于为部分文本设置样式属性。

```HTML
<span>这是一个span标签</span>
```



### 12.表单

表单是一个包含表单元素的区域。

表单元素是允许用户在表单中输入内容,比如：文本域(textarea)、下拉列表、单选框(radio-buttons)、复选框(checkboxes)等等。

表单使用表单标签 <form> 来设置:

```HTML
<form>
表单
</form>
```

###### action：表单提交地址

###### method:  表单提交方式



#### 1.input 输入元素

多数情况下被用到的表单标签是输入标签（<input>）。

输入类型是由类型属性（type）定义的。大多数经常被用到的输入类型如下：

##### 1.文本域（text）

文本域通过<input type="text"> 标签来设定，当用户要在表单中键入字母、数字等内容时，就会用到文本域。

```HTML
<form action="提交地址" method="get">
账号: <input type="text" name="username"><br>
</form>
```

##### 2.密码 （password）

密码字段通过标签<input type="password"> 来定义:

```HTML
<form>
密码: <input type="password" name="pwd">
</form>
```

##### 3.单选框（radio）

<input type="radio"> 标签定义了表单单选框选项

```HTML
<form>
<input type="radio" name="sex" value="1">男
<input type="radio" name="sex" value="2">女
</form>
```

##### 4.复选框（checkbox）

<input type="checkbox"> 定义了复选框. 用户需要从若干给定的选择中选取一个或若干选项。

```HTML
<form>
<input type="checkbox" name="type" value="Bike">篮球
<input type="checkbox" name="type" value="Car">足球
</form>
```

##### 5.提交按钮 （submit）

<input type="submit"> 定义了提交按钮.

当用户单击确认按钮时，表单的内容会被传送到另一个文件。表单的动作属性定义了目的文件的文件名。由动作属性定义的这个文件通常会对接收到的输入数据进行相关的处理

```HTML
<form>
账号: <input type="text" name="user">
<input type="submit" value="提交">
</form>
```

##### 6.输入属性

###### readonly：只读

###### disabled ：禁用

###### maxlength： 规定输入字段允许的最大长度



#### 2.select下拉列表

*<select>* 元素定义下拉列表

*<option>* 元素定义待选择的选项。

列表通常会把首个选项显示为被选选项。

您能够通过添加 selected 属性来定义预定义选项。

```
<select name="cars">
<option selected value="1">选项1</option>
<option value="2">选项2</option>
<option value="3">选项3</option>
<option value="4">选项4</option>
</select>
```



#### 3.textarea 文本域

*<textarea>* 元素定义多行输入字段，并且可以通过**rows**以及**cols**设置宽高

```HTML
<textarea name="message" rows="10" cols="30">
这是一个文本域
</textarea>
```



#### 4.button

*<button>* 元素定义可点击的按钮

```
<button type="button">提交</button>
```



### 13.框架

过使用框架**iframe**，你可以在同一个浏览器窗口中显示不止一个页面

```html
<iframe src="https://www.baidu.com/"></iframe>
```

​	height 和 width 属性用来定义iframe标签的高度与宽度。

属性默认以像素为单位, 但是你可以指定其按比例显示 (如："80%")

```html
<iframe width="80%" height="200" src="https://www.baidu.com/"></iframe>
```



## HTML事件

可以使 HTML 事件触发浏览器中的行为，比方说当用户点击某个 HTML 元素时启动一段 JavaScript。

#### 1.表单事件(Form Events)

表单事件在HTML表单中触发 (适用于所有 HTML 元素, 但该HTML元素需在form表单内):

| 属性     | 值       | 描述                                  |
| :------- | :------- | :------------------------------------ |
| onblur   | *script* | 当元素失去焦点时运行脚本              |
| onchange | *script* | 当元素改变时运行脚本                  |
| onfocus  | *script* | 当元素获得焦点时运行脚本              |
| onreset  | *script* | 当表单重置时运行脚本。HTML 5 不支持。 |
| onselect | *script* | 当选取元素时运行脚本                  |
| onsubmit | *script* | 当提交表单时运行脚本                  |



#### 2.键盘事件（Keyboard Events）

| 属性       | 值       | 描述                       |
| :--------- | :------- | :------------------------- |
| onkeydown  | *script* | 当按下按键时运行脚本       |
| onkeypress | *script* | 当按下并松开按键时运行脚本 |
| onkeyup    | *script* | 当松开按键时运行脚本       |



#### 3.鼠标事件（Mouse Events）

通过鼠标触发事件, 类似用户的行为:

| 属性        | 值       | 描述                             |
| :---------- | :------- | :------------------------------- |
| onclick     | *script* | 当单击鼠标时运行脚本             |
| ondblclick  | *script* | 当双击鼠标时运行脚本             |
| onmousedown | *script* | 当按下鼠标按钮时运行脚本         |
| onmousemove | *script* | 当鼠标指针移动时运行脚本         |
| onmouseout  | *script* | 当鼠标指针移出元素时运行脚本     |
| onmouseover | *script* | 当鼠标指针移至元素之上时运行脚本 |
| onmouseup   | *script* | 当松开鼠标按钮时运行脚本         |

