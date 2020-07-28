1、`<mata>`标签
--

`<meta>`元素可提供有关页面的元信息，比如针对搜索引擎和更新频度的描述和关键词。它位于文档的头部，不包含任何内容，定义了与文档相关联的名称/值对。

`name`属性提供了名称/值对中的名称。`HTML` 和 `XHTML` 标签都没有指定任何预先定义的 `<meta>` 名称。通常情况下，您可以自由使用对自己和源文档的读者来说富有意义的名称。如果没有提供 `name` 属性，那么名称/值对中的名称会采用 `http-equiv` 属性的值。

`content`属性提供了名称/值对中的值。该值可以是任何有效的字符串。它始终要和 `name` 属性或 `http-equiv` 属性一起使用。

注释：`<meta>`标签永远位于`head`元素内部，元素总是以名称/值的形式被成对传递。

2、`<link>`标签
--

链接一个外部样式表。仅出现与`head`部分，不过可以出现任何次。

常见属性：
* href：规定被链接文档的位置。
* rel：规定当前文档与被链接文档之间的关系。
* type：规定被链接文档的MIME类型。

3、`<img>`标签
--

`<img>`元素向网页中嵌入一幅图像。请注意，从技术上讲，`<img>` 标签并不会在网页中插入图像，而是从网页上链接图像。`<img>` 标签创建的是被引用图像的占位空间。

两个必需的属性：`src`和`alt`属性。

常用属性：
* src：规定显示图像的URL。
* alt：规定图像的替代文本。

4、`<div>`属性
--

可定义文档中的分区或节。`<div>`标签可以把文档分割为独立的、不同的部分。它可以用作严格的组织工具，并且不使用任何格式与其关联，如果用`id`和`class`来标记`<div>`，那么该标签的作用会变得更加有效。

用法：`<div>`是一个块级元素。这意味着它的内容自动地开始一个新行。实际上，换行是 `<div>` 固有的唯一格式表现。可以通过 `<div>` 的 `class` 或 `id` 应用额外的样式。不必为每一个 `<div>` 都加上类或 `id`，虽然这样做也有一定的好处。可以对同一个 `<div>` 元素应用 `class` 或 `id` 属性，但是更常见的情况是只应用其中一种。这两者的主要差异是，`class` 用于元素组（类似的元素，或者可以理解为某一类元素），而 `id` 用于标识单独的唯一的元素。

5、`<ul>`标签
--

`<ul>`标签定义无序列表。

属性：
* class：规定元素的类名。
* id：规定元素的唯一id。
* style：规定元素的行内样式。
* title：规定元素的额外信息。

6、body{}用途
--

`html{background-color:white;}`浏览器能看到的所有范围 ，不包括边框。`body{background-color:green;}`与`html`一样，浏览器能看到的所有访问但无像`html`一样包括边框,级别`html>body`。

eg:
###
    <head>
    <meta http-equiv="Content-Type" content="text/html; charset=gb2312" />
    <title>无标题文档</title>
      <style>
           html{
                 background-color:red;
          }
          body{
                 background-color:blue;
          }
           .div1{
             background-color:green;
             width:222px;
            height:440px;  
          }    
      </style>
    
    </head>

上述代码效果：
![Image text](https://github.com/dp9527/JavaWeb/blob/master/body%7B%7D%E6%95%88%E6%9E%9C%E5%9B%BE.jpg)

注：div中的px代表的是像素，是相对于屏幕分辨率来说的。














