FreeCodeCamp - Responsive Design with Bootstrap
（转载）（
作者：付林恒
链接：https://www.jianshu.com/p/a44a5aa4eca1
來源：简书
著作权归作者所有。商业转载请联系作者获得授权，非商业转载请注明出处。）
Use Responsive Design with Bootstrap Fluid Containers
现在让我们回到我们的Cat Photo应用。这次，我们将用流行的响应式框架Bootstrap来美化它。

Bootstrap将会根据你的屏幕的大小来调整HTML元素的大小 —— 强调 响应式设计的概念。

通过响应式设计，你无需再为你的网站设计一个手机版的。它在任何尺寸的屏幕上看起来都会不错。

你仅需要通过添加下列代码到你的HTML开头来将Bootstrap添加到任意应用中：

<link rel="stylesheet" href="//cdn.bootcss.com/bootstrap/3.3.1/css/bootstrap.min.css"/>

在此案例中，我们已经帮你把上述代码添加到页面中。

首先，我们需要把所有的HTML内容放在class为container-fluid的div下。

<link href="//fonts.gdgdocs.org/css?family=Lobster" rel="stylesheet" type="text/css">
<style>
.red-text {
color: red;
}

h2 {
font-family: Lobster, Monospace;
}

p {
font-size: 16px;
font-family: Monospace;
}

.thick-green-border {
border-color: green;
border-width: 10px;
border-style: solid;
border-radius: 50%;
}

.smaller-image {
width: 100px;
}
</style>
<div class="container-fluid">
<h2 class="red-text">CatPhotoApp</h2>

<p>Click here for <a href="#">cat photos</a>.</p>

<a href="#">![](/images/relaxing-cat.jpg)</a>

<p>Things cats love:</p>
<ul>
<li>cat nip</li>
<li>laser pointers</li>
<li>lasagna</li>
</ul>
<p>Top 3 things cats hate:</p>
<ol>
<li>flea treatment</li>
<li>thunder</li>
<li>other cats</li>
</ol>
<form action="/submit-cat-photo">
<label><input type="radio" name="indoor-outdoor"> Indoor</label>
<label><input type="radio" name="indoor-outdoor"> Outdoor</label>
<label><input type="checkbox" name="personality"> Loving</label>
<label><input type="checkbox" name="personality"> Lazy</label>
<label><input type="checkbox" name="personality"> Crazy</label>
<input type="text" placeholder="cat photo URL" required>
<button type="submit">Submit</button>
</form>
</div>
Make Images Mobile Responsive
首先，在已有的图片下方添加一张新的图片。将它的 src属性设置为 /images/running-cat.jpg。

如果图片的尺寸刚好等于我们手机的尺寸，那想必是极好的。

谢天谢地，通过Bootstrap，我们要做的只是给图片添加 img-responsive class属性。这样图片的宽度就能完美地适配你的页面的宽度了。

<link href="//fonts.gdgdocs.org/css?family=Lobster" rel="stylesheet" type="text/css">
<style>
.red-text {
color: red;
}

h2 {
font-family: Lobster, Monospace;
}

p {
font-size: 16px;
font-family: Monospace;
}

.thick-green-border {
border-color: green;
border-width: 10px;
border-style: solid;
border-radius: 50%;
}

.smaller-image {
width: 100px;
}
</style>

<div class="container-fluid">
<h2 class="red-text">CatPhotoApp</h2>

<p>Click here for <a href="#">cat photos</a>.</p>

<a href="#">![](/images/relaxing-cat.jpg)</a>
![](/images/running-cat.jpg)
<p>Things cats love:</p>
<ul>
<li>cat nip</li>
<li>laser pointers</li>
<li>lasagna</li>
</ul>
<p>Top 3 things cats hate:</p>
<ol>
<li>flea treatment</li>
<li>thunder</li>
<li>other cats</li>
</ol>
<form action="/submit-cat-photo">
<label><input type="radio" name="indoor-outdoor"> Indoor</label>
<label><input type="radio" name="indoor-outdoor"> Outdoor</label>
<label><input type="checkbox" name="personality"> Loving</label>
<label><input type="checkbox" name="personality"> Lazy</label>
<label><input type="checkbox" name="personality"> Crazy</label>
<input type="text" placeholder="cat photo URL" required>
<button type="submit">Submit</button>
</form>
</div>

Center Text with Bootstrap
既然我们在使用Bootstrap，我们可以通过居中头部元素来使它看起来更棒。 我们所要做的只是把text-center class属性添加给 h2 元素。

记住：你可以用空格分开多个class来为同一个元素添加多个 class 属性， 就像这样：

<h2 class="red-text text-center">your text</h2>

<link href="//fonts.gdgdocs.org/css?family=Lobster" rel="stylesheet" type="text/css">
<style>
.red-text {
color: red;
}

h2 {
font-family: Lobster, Monospace;
}

p {
font-size: 16px;
font-family: Monospace;
}

.thick-green-border {
border-color: green;
border-width: 10px;
border-style: solid;
border-radius: 50%;
}

.smaller-image {
width: 100px;
}
</style>

<div class="container-fluid">
<h2 class="red-text text-center">CatPhotoApp</h2>

<p>Click here for <a href="#">cat photos</a>.</p>

<a href="#">![](/images/relaxing-cat.jpg)</a>

![](/images/running-cat.jpg)
<p>Things cats love:</p>
<ul>
<li>cat nip</li>
<li>laser pointers</li>
<li>lasagna</li>
</ul>
<p>Top 3 things cats hate:</p>
<ol>
<li>flea treatment</li>
<li>thunder</li>
<li>other cats</li>
</ol>
<form action="/submit-cat-photo">
<label><input type="radio" name="indoor-outdoor"> Indoor</label>
<label><input type="radio" name="indoor-outdoor"> Outdoor</label>
<label><input type="checkbox" name="personality"> Loving</label>
<label><input type="checkbox" name="personality"> Lazy</label>
<label><input type="checkbox" name="personality"> Crazy</label>
<input type="text" placeholder="cat photo URL" required>
<button type="submit">Submit</button>
</form>
</div>

Create a Bootstrap Button
Bootstrap有它自己的 button 按钮风格， 看起来要比默认的按钮好看得多。

在三只猫咪图片下面创建一个新的 button 元素。给它添加 btn class 属性以及"Like"文本。

<link href="//fonts.gdgdocs.org/css?family=Lobster" rel="stylesheet" type="text/css">
<style>
.red-text {
color: red;
}

h2 {
font-family: Lobster, Monospace;
}

p {
font-size: 16px;
font-family: Monospace;
}

.thick-green-border {
border-color: green;
border-width: 10px;
border-style: solid;
border-radius: 50%;
}

.smaller-image {
width: 100px;
}
</style>

<div class="container-fluid">
<h2 class="red-text text-center">CatPhotoApp</h2>

<p>Click here for <a href="#">cat photos</a>.</p>

<a href="#">![](/images/relaxing-cat.jpg)</a>

![](/images/running-cat.jpg)
<button class="btn">like</button>
<p>Things cats love:</p>
<ul>
<li>cat nip</li>
<li>laser pointers</li>
<li>lasagna</li>
</ul>
<p>Top 3 things cats hate:</p>
<ol>
<li>flea treatment</li>
<li>thunder</li>
<li>other cats</li>
</ol>
<form action="/submit-cat-photo">
<label><input type="radio" name="indoor-outdoor"> Indoor</label>
<label><input type="radio" name="indoor-outdoor"> Outdoor</label>
<label><input type="checkbox" name="personality"> Loving</label>
<label><input type="checkbox" name="personality"> Lazy</label>
<label><input type="checkbox" name="personality"> Crazy</label>
<input type="text" placeholder="cat photo URL" required>
<button type="submit">Submit</button>
</form>
</div>

Create a Block Element Bootstrap Button
通常情况下，你的 button 元素仅与它所包含的文本一样宽。通过使其成为块级元素，你的按钮将会伸展并填满页面整个水平空间，任何在它之下的元素都会跟着浮动至该区块的下一行。

这张图阐述了行内元素与块级元素的区别：


An
注意，这些按钮仍然需要 btn class。

添加Bootstrap的 btn-block class 到你的按钮。

<link href="//fonts.gdgdocs.org/css?family=Lobster" rel="stylesheet" type="text/css">
<style>
.red-text {
color: red;
}

h2 {
font-family: Lobster, Monospace;
}

p {
font-size: 16px;
font-family: Monospace;
}

.thick-green-border {
border-color: green;
border-width: 10px;
border-style: solid;
border-radius: 50%;
}

.smaller-image {
width: 100px;
}
</style>

<div class="container-fluid">
<h2 class="red-text text-center">CatPhotoApp</h2>

<p>Click here for <a href="#">cat photos</a>.</p>

<a href="#">![](/images/relaxing-cat.jpg)</a>

![](/images/running-cat.jpg)
<button class="btn btn-block">Like</button>
<p>Things cats love:</p>
<ul>
<li>cat nip</li>
<li>laser pointers</li>
<li>lasagna</li>
</ul>
<p>Top 3 things cats hate:</p>
<ol>
<li>flea treatment</li>
<li>thunder</li>
<li>other cats</li>
</ol>
<form action="/submit-cat-photo">
<label><input type="radio" name="indoor-outdoor"> Indoor</label>
<label><input type="radio" name="indoor-outdoor"> Outdoor</label>
<label><input type="checkbox" name="personality"> Loving</label>
<label><input type="checkbox" name="personality"> Lazy</label>
<label><input type="checkbox" name="personality"> Crazy</label>
<input type="text" placeholder="cat photo URL" required>
<button type="submit">Submit</button>
</form>
</div>

Taste the Bootstrap Button Color Rainbow
深蓝色btn-primary是你的应用的主要颜色，被用在那些用户主要采取的操作上。

添加Bootstrap的 btn-primary class 属性到按钮标签上。

注意：这个按钮仍然需要 btn 和 btn-block 属性！

<link href="//fonts.gdgdocs.org/css?family=Lobster" rel="stylesheet" type="text/css">
<style>
.red-text {
color: red;
}

h2 {
font-family: Lobster, Monospace;
}

p {
font-size: 16px;
font-family: Monospace;
}

.thick-green-border {
border-color: green;
border-width: 10px;
border-style: solid;
border-radius: 50%;
}

.smaller-image {
width: 100px;
}
</style>

<div class="container-fluid">
<h2 class="red-text text-center">CatPhotoApp</h2>

<p>Click here for <a href="#">cat photos</a>.</p>

<a href="#">![](/images/relaxing-cat.jpg)</a>

![](/images/running-cat.jpg)
<button class="btn btn-block btn-primary">Like</button>
<p>Things cats love:</p>
<ul>
<li>cat nip</li>
<li>laser pointers</li>
<li>lasagna</li>
</ul>
<p>Top 3 things cats hate:</p>
<ol>
<li>flea treatment</li>
<li>thunder</li>
<li>other cats</li>
</ol>
<form action="/submit-cat-photo">
<label><input type="radio" name="indoor-outdoor"> Indoor</label>
<label><input type="radio" name="indoor-outdoor"> Outdoor</label>
<label><input type="checkbox" name="personality"> Loving</label>
<label><input type="checkbox" name="personality"> Lazy</label>
<label><input type="checkbox" name="personality"> Crazy</label>
<input type="text" placeholder="cat photo URL" required>
<button type="submit">Submit</button>
</form>
</div>

Call out Optional Actions with Button Info
Bootstrap自带了一些预定义的按钮颜色。浅蓝色 btn-info被用在那些用户可能会采取的操作上。

在你的 "Like" 按钮下面添加一个文本为 "Info" 的块级Bootstrap按钮，并为其添加 btn-info 和 btn-block class属性。

注意：这些按钮仍然需要 btn 和 btn-block class属性

<link href="//fonts.gdgdocs.org/css?family=Lobster" rel="stylesheet" type="text/css">
<style>
.red-text {
color: red;
}

h2 {
font-family: Lobster, Monospace;
}

p {
font-size: 16px;
font-family: Monospace;
}

.thick-green-border {
border-color: green;
border-width: 10px;
border-style: solid;
border-radius: 50%;
}

.smaller-image {
width: 100px;
}
</style>

<div class="container-fluid">
<h2 class="red-text text-center">CatPhotoApp</h2>

<p>Click here for <a href="#">cat photos</a>.</p>

<a href="#">![](/images/relaxing-cat.jpg)</a>

![](/images/running-cat.jpg)
<button class="btn btn-block btn-primary">Like</button>
<button class="btn btn-block btn-info">Info</button>
<p>Things cats love:</p>
<ul>
<li>cat nip</li>
<li>laser pointers</li>
<li>lasagna</li>
</ul>
<p>Top 3 things cats hate:</p>
<ol>
<li>flea treatment</li>
<li>thunder</li>
<li>other cats</li>
</ol>
<form action="/submit-cat-photo">
<label><input type="radio" name="indoor-outdoor"> Indoor</label>
<label><input type="radio" name="indoor-outdoor"> Outdoor</label>
<label><input type="checkbox" name="personality"> Loving</label>
<label><input type="checkbox" name="personality"> Lazy</label>
<label><input type="checkbox" name="personality"> Crazy</label>
<input type="text" placeholder="cat photo URL" required>
<button type="submit">Submit</button>
</form>
</div>

Warn your Users of a Dangerous Action
Bootstrap自带了一些预定义的按钮颜色。红色btn-danger被用来提醒用户该操作具有“破坏性”，例如删除一张猫的图片。

创建一个文本为 "Delete" 的按钮，并且给它添加 class btn-danger。

注意：这些标签仍然需要 btn 与 btn-block class。

<link href="//fonts.gdgdocs.org/css?family=Lobster" rel="stylesheet" type="text/css">
<style>
.red-text {
color: red;
}

h2 {
font-family: Lobster, Monospace;
}

p {
font-size: 16px;
font-family: Monospace;
}

.thick-green-border {
border-color: green;
border-width: 10px;
border-style: solid;
border-radius: 50%;
}

.smaller-image {
width: 100px;
}
</style>

<div class="container-fluid">
<h2 class="red-text text-center">CatPhotoApp</h2>

<p>Click here for <a href="#">cat photos</a>.</p>

<a href="#">![](/images/relaxing-cat.jpg)</a>

![](/images/running-cat.jpg)
<button class="btn btn-block btn-primary">Like</button>
<button class="btn btn-block btn-info">Info</button>
<button class="btn btn-block btn-danger">Delete</button>
<p>Things cats love:</p>
<ul>
<li>cat nip</li>
<li>laser pointers</li>
<li>lasagna</li>
</ul>
<p>Top 3 things cats hate:</p>
<ol>
<li>flea treatment</li>
<li>thunder</li>
<li>other cats</li>
</ol>
<form action="/submit-cat-photo">
<label><input type="radio" name="indoor-outdoor"> Indoor</label>
<label><input type="radio" name="indoor-outdoor"> Outdoor</label>
<label><input type="checkbox" name="personality"> Loving</label>
<label><input type="checkbox" name="personality"> Lazy</label>
<label><input type="checkbox" name="personality"> Crazy</label>
<input type="text" placeholder="cat photo URL" required>
<button type="submit">Submit</button>
</form>
</div>

Use the Bootstrap Grid to Put Elements Side By Side
Bootstrap 使用一种响应式网格布局——可轻松实现将多个元素放入一行并指定各个元素的相对宽度的需求。Bootstrap 中大多数的class属性都可以设置于 div 元素中。

下面这张图表显示了 Bootstraps 的12列网格布局是如何起作用的：


an image illustrating Bootstrap's grid system
请注意，在这张图表中，class属性 col-md-* 正被使用。在这里，md 表示 medium (中等的)，* 代表一个数字，它指定了这个元素所占的列宽。通过此图表的属性设置可知，在中等大小的屏幕上(例如笔记本电脑)，元素的列宽被指定了。

在我们创建的 Cat Photo App 中，将会使用 col-xs-*，其中 xs 是 extra small 缩写（应用于较小的屏幕，比如手机屏幕），* 是你需要填写的数字，代表在一行中,各个元素应该占的列宽。

把 Like, Info 和 Delete 三个按钮一并放入一个 <div class="row"> 元素中；然后，其中的每一个按钮都需要各自被一个 <div class="col-xs-4"> 元素包裹。

当div 元素设置了 class 属性 row 之后，那几个按钮便可嵌入其中。

<link href="//fonts.gdgdocs.org/css?family=Lobster" rel="stylesheet" type="text/css">
<style>
.red-text {
color: red;
}

h2 {
font-family: Lobster, Monospace;
}

p {
font-size: 16px;
font-family: Monospace;
}

.thick-green-border {
border-color: green;
border-width: 10px;
border-style: solid;
border-radius: 50%;
}

.smaller-image {
width: 100px;
}
</style>

<div class="container-fluid">
<h2 class="red-text text-center">CatPhotoApp</h2>

<p>Click here for <a href="#">cat photos</a>.</p>

<a href="#">![](/images/relaxing-cat.jpg)</a>

![](/images/running-cat.jpg)
<div class="row">
<div class=" col-xs-4"><button class="btn btn-block btn-primary">Like</button></div>
<div class=" col-xs-4"><button class="btn btn-block btn-info">Info</button></div>
<div class=" col-xs-4"><button class="btn btn-block btn-danger">Delete</button></div>
</div>
<p>Things cats love:</p>
<ul>
<li>cat nip</li>
<li>laser pointers</li>
<li>lasagna</li>
</ul>
<p>Top 3 things cats hate:</p>
<ol>
<li>flea treatment</li>
<li>thunder</li>
<li>other cats</li>
</ol>
<form action="/submit-cat-photo">
<label><input type="radio" name="indoor-outdoor"> Indoor</label>
<label><input type="radio" name="indoor-outdoor"> Outdoor</label>
<label><input type="checkbox" name="personality"> Loving</label>
<label><input type="checkbox" name="personality"> Lazy</label>
<label><input type="checkbox" name="personality"> Crazy</label>
<input type="text" placeholder="cat photo URL" required>
<button type="submit">Submit</button>
</form>
</div>

Ditch Custom CSS for Bootstrap
现在，让我们清理一下之前的代码了，以让我们的 Cat Photo 应用看起来更简洁，用 Bootstrap 内置的样式来替换我们之前自定义的样式。

别担心 —— 以后我们会有大把时间来自定义我们的 CSS 样式的 ：）

删除 style 元素里的 .red-text, p 和 .smaller-imageCSS声明，这样你的 style 留下的声明就只有 h2 和 thick-green-border。

然后删除包含死链接的 p 元素。 移除 h2 元素的 red-text class 并且用 Bootstrap的 text-primary class替换之。

最后，移除第一个 img 元素的 "smaller -image" class ，替换为 Bootstrap的 img-responsive class。

<link href="//fonts.gdgdocs.org/css?family=Lobster" rel="stylesheet" type="text/css">
<style>
.red-text {
color: red;
}

h2 {
font-family: Lobster, Monospace;
}

p {
font-size: 16px;
}

.thick-green-border {
border-color: green;
border-width: 10px;
border-style: solid;
border-radius: 50%;
}
</style>

<div class="container-fluid">
<h2 class="text-center text-primary">CatPhotoApp</h2>

<p>Click here for <a href="#">cat photos</a>.</p>

<a href="#">![](/images/relaxing-cat.jpg)</a>

![](/images/running-cat.jpg)
<div class="row">
<div class="col-xs-4">
<button class="btn btn-block btn-primary">Like</button>
</div>
<div class="col-xs-4">
<button class="btn btn-block btn-info">Info</button>
</div>
<div class="col-xs-4">
<button class="btn btn-block btn-danger">Delete</button>
</div>
</div>
<p>Things cats love:</p>
<ul>
<li>cat nip</li>
<li>laser pointers</li>
<li>lasagna</li>
</ul>
<p>Top 3 things cats hate:</p>
<ol>
<li>flea treatment</li>
<li>thunder</li>
<li>other cats</li>
</ol>
<form action="/submit-cat-photo">
<label><input type="radio" name="indoor-outdoor"> Indoor</label>
<label><input type="radio" name="indoor-outdoor"> Outdoor</label>
<label><input type="checkbox" name="personality"> Loving</label>
<label><input type="checkbox" name="personality"> Lazy</label>
<label><input type="checkbox" name="personality"> Crazy</label>
<input type="text" placeholder="cat photo URL" required>
<button type="submit">Submit</button>
</form>
</div>

Use Spans for Inline Elements
你可以用 span 标签来创建行内元素。还记得我们是怎样使用 .btn-block来创建填满整行的按钮吗？

这张图展示了 inline 元素与 block-level 块级元素的区别：


An
通过使用 span 元素，你可以把几个元素放在一起。你甚至可以用此为一个元素的不同部分指定样式。

把 "Things cats love" 中的 "love" 放到 span 标签下。然后为其添加 text-danger class 来使文字变成红色。

举例，"Top 3 things cats hate" 元素的写法如下：

<p>Top 3 things cats <span class = "text-danger">hate:</span></p>

<link href="//fonts.gdgdocs.org/css?family=Lobster" rel="stylesheet" type="text/css">
<style>

h2 {
font-family: Lobster, Monospace;
}

.thick-green-border {
border-color: green;
border-width: 10px;
border-style: solid;
border-radius: 50%;
}

</style>

<div class="container-fluid">
<h2 class="text-primary text-center">CatPhotoApp</h2>

<a href="#">![](/images/relaxing-cat.jpg)</a>

![](/images/running-cat.jpg)
<div class="row">
<div class="col-xs-4">
<button class="btn btn-block btn-primary">Like</button>
</div>
<div class="col-xs-4">
<button class="btn btn-block btn-info">Info</button>
</div>
<div class="col-xs-4">
<button class="btn btn-block btn-danger">Delete</button>
</div>
</div>
<p><span class="text-danger">Things cats love:</span></p>
<ul>
<li>cat nip</li>
<li>laser pointers</li>
<li>lasagna</li>
</ul>
<p>Top 3 things cats hate:</p>
<ol>
<li>flea treatment</li>
<li>thunder</li>
<li>other cats</li>
</ol>
<form action="/submit-cat-photo">
<label><input type="radio" name="indoor-outdoor"> Indoor</label>
<label><input type="radio" name="indoor-outdoor"> Outdoor</label>
<label><input type="checkbox" name="personality"> Loving</label>
<label><input type="checkbox" name="personality"> Lazy</label>
<label><input type="checkbox" name="personality"> Crazy</label>
<input type="text" placeholder="cat photo URL" required>
<button type="submit">Submit</button>
</form>
</div>

Create a Custom Heading
让我们来为Cat Photo 应用做一个导航吧，把标题和惬意的猫图片放在同一行。

记住，Bootstrap使用响应式栅格系统，这使得把元素放入行内并为每个元素指定宽度变得很容易。大部分的 Bootstrap的 class 都可以被用在 div 元素上。

这张图展示了 Bootstrap 的12栏栅格布局是如何工作的：


an image illustrating Bootstrap's grid system
注意，在此图示中，我们使用了 col-md-* class 。此处 md 代表中等，* 指定了元素宽度应该占用的栏数。 在这个案例中，我们指定了元素在中等大小的屏幕（如笔记本等）上所占用的栏数。

在此应用中，我们将使用 col-xs-*， xs 意味着非常小（比如非常小的手机屏幕）， * 指定了元素宽度应该占用的栏数。

将你的第一张图片和 h2 元素放到同一个 <div class="row"> 元素下。 将你的 h2 元素放到 <div class="col-xs-8"> 下，你的图片放到 <div class="col-xs-4"> 下，这样他们就能位于同一行了。

注意现在图片是否与文字大小一致呢？

<link href="//fonts.gdgdocs.org/css?family=Lobster" rel="stylesheet" type="text/css">

<style>
h2 {
font-family: Lobster, Monospace;
}

.thick-green-border {
border-color: green;
border-width: 10px;
border-style: solid;
border-radius: 50%;
}
</style>

<div class="container-fluid">
<div class="row">
<div class="col-xs-8">
<h2 class="text-primary text-center">CatPhotoApp</h2>
</div>
<div class="col-xs-4">
<a href="#">![](/images/relaxing-cat.jpg)</a>
</div>
</div>
![](/images/running-cat.jpg)
<div class="row">
<div class="col-xs-4">
<button class="btn btn-block btn-primary">Like</button>
</div>
<div class="col-xs-4">
<button class="btn btn-block btn-info">Info</button>
</div>
<div class="col-xs-4">
<button class="btn btn-block btn-danger">Delete</button>
</div>
</div>
<p>Things cats <span class="text-danger">love:</span></p>
<ul>
<li>cat nip</li>
<li>laser pointers</li>
<li>lasagna</li>
</ul>
<p>Top 3 things cats hate:</p>
<ol>
<li>flea treatment</li>
<li>thunder</li>
<li>other cats</li>
</ol>
<form action="/submit-cat-photo">
<label><input type="radio" name="indoor-outdoor"> Indoor</label>
<label><input type="radio" name="indoor-outdoor"> Outdoor</label>
<label><input type="checkbox" name="personality"> Loving</label>
<label><input type="checkbox" name="personality"> Lazy</label>
<label><input type="checkbox" name="personality"> Crazy</label>
<input type="text" placeholder="cat photo URL" required>
<button type="submit">Submit</button>
</form>
</div>

Add Font Awesome Icons to our Buttons
Font Awesome 是一个非常方便的图标库。这些图标都是矢量图形，被保存在 .svg 的文件格式中。这些图标就和字体一样，你可以通过像素单位指定它们的大小，它们将会继承其父HTML元素的字体大小。

你可以将 Font Awesome 图标库增添至任何一个应用中，方法很简单，只需要在你的 HTML 头部增加下列代码即可：

<link rel="stylesheet" href="//cdn.bootcss.com/font-awesome/4.2.0/css/font-awesome.min.css"/>

不过，我们已经事先在幕后为此页面添加了该功能。（不必重复添加上面这段代码）

i 元素起初一般是让其它元素有斜体(italic)的功能，不过现在一般用来指代图标。你可以将 Font Awesome 中的 class 属性添加到 i 元素中，把它变成一个图标，比如：

<i class="fa fa-info-circle"></i>

你可以通过 Font Awesome 库增加一个 thumbs-up 图标到你的 like 按钮中，方法是在i 元素中增加 class 属性 fa 和 fa-thumbs-up。

<link href="//fonts.gdgdocs.org/css?family=Lobster" rel="stylesheet" type="text/css">
<style>
h2 {
font-family: Lobster, Monospace;
}

.thick-green-border {
border-color: green;
border-width: 10px;
border-style: solid;
border-radius: 50%;
}
</style>

<div class="container-fluid">
<div class="row">
<div class="col-xs-8">
<h2 class="text-primary text-center">CatPhotoApp</h2>
</div>
<div class="col-xs-4">
<a href="#">![](/images/relaxing-cat.jpg)</a>
</div>
</div>
![](/images/running-cat.jpg)
<div class="row">
<div class="col-xs-4">
<button class="btn btn-block btn-primary">Like<i class="fa fa-thumbs-up"></i></button>
</div>
<div class="col-xs-4">
<button class="btn btn-block btn-info">Info</button>
</div>
<div class="col-xs-4">
<button class="btn btn-block btn-danger">Delete</button>
</div>
</div>
<p>Things cats <span class="text-danger">love:</span></p>
<ul>
<li>cat nip</li>
<li>laser pointers</li>
<li>lasagna</li>
</ul>
<p>Top 3 things cats hate:</p>
<ol>
<li>flea treatment</li>
<li>thunder</li>
<li>other cats</li>
</ol>
<form action="/submit-cat-photo">
<label><input type="radio" name="indoor-outdoor"> Indoor</label>
<label><input type="radio" name="indoor-outdoor"> Outdoor</label>
<label><input type="checkbox" name="personality"> Loving</label>
<label><input type="checkbox" name="personality"> Lazy</label>
<label><input type="checkbox" name="personality"> Crazy</label>
<input type="text" placeholder="cat photo URL" required>
<button type="submit">Submit</button>
</form>
</div>

Add Font Awesome Icons to all of our Buttons
Font Awesome 是一个非常方便的图标库。这些图片都是矢量图，以 .svg 文件格式保存。这些图标用起来就像字体一样。你可以使用像素单位来指定他们的大小，它们会继承父级HTML元素的字体大小。

使用 Font Awesome 分别为你的 info 按钮添加 info-circle 图标，为你的 delete 按钮添加 trash 图标。

<link href="//fonts.gdgdocs.org/css?family=Lobster" rel="stylesheet" type="text/css">
<style>
h2 {
font-family: Lobster, Monospace;
}

.thick-green-border {
border-color: green;
border-width: 10px;
border-style: solid;
border-radius: 50%;
}
</style>

<div class="container-fluid">
<div class="row">
<div class="col-xs-8">
<h2 class="text-primary text-center">CatPhotoApp</h2>
</div>
<div class="col-xs-4">
<a href="#">![](/images/relaxing-cat.jpg)</a>
</div>
</div>
![](/images/running-cat.jpg)
<div class="row">
<div class="col-xs-4">
<button class="btn btn-block btn-primary"><i class="fa fa-thumbs-up"></i> Like</button>
</div>
<div class="col-xs-4">
<button class="btn btn-block btn-info"><i class="fa fa-info-circle"></i>Info</button>
</div>
<div class="col-xs-4">
<button class="btn btn-block btn-danger"><i class="fa fa-trash"></i>Delete</button>
</div>
</div>
<p>Things cats <span class="text-danger">love:</span></p>
<ul>
<li>cat nip</li>
<li>laser pointers</li>
<li>lasagna</li>
</ul>
<p>Top 3 things cats hate:</p>
<ol>
<li>flea treatment</li>
<li>thunder</li>
<li>other cats</li>
</ol>
<form action="/submit-cat-photo">
<label><input type="radio" name="indoor-outdoor"> Indoor</label>
<label><input type="radio" name="indoor-outdoor"> Outdoor</label>
<label><input type="checkbox" name="personality"> Loving</label>
<label><input type="checkbox" name="personality"> Lazy</label>
<label><input type="checkbox" name="personality"> Crazy</label>
<input type="text" placeholder="cat photo URL" required>
<button type="submit">Submit</button>
</form>
</div>

Responsively Style Radio Buttons
你还可以将 Bootstrap 的 col-xs-*用在 form 元素中。这样的话，我们的单选按钮就可以均匀地在页面上展开，不需要知道屏幕的分辨率有多宽。

将页面中的两个单选按钮放置于一个 <div class="row">元素中。然后，添加 <div class="col-xs-6"> 元素并分别包裹每一个单选按钮。

<link href="//fonts.gdgdocs.org/css?family=Lobster" rel="stylesheet" type="text/css">
<style>
h2 {
font-family: Lobster, Monospace;
}

.thick-green-border {
border-color: green;
border-width: 10px;
border-style: solid;
border-radius: 50%;
}
</style>

<div class="container-fluid">
<div class="row">
<div class="col-xs-8">
<h2 class="text-primary text-center">CatPhotoApp</h2>
</div>
<div class="col-xs-4">
<a href="#">![](/images/relaxing-cat.jpg)</a>
</div>
</div>
![](/images/running-cat.jpg)
<div class="row">
<div class="col-xs-4">
<button class="btn btn-block btn-primary"><i class="fa fa-thumbs-up"></i> Like</button>
</div>
<div class="col-xs-4">
<button class="btn btn-block btn-info"><i class="fa fa-info-circle"></i> Info</button>
</div>
<div class="col-xs-4">
<button class="btn btn-block btn-danger"><i class="fa fa-trash"></i> Delete</button>
</div>
</div>
<p>Things cats <span class="text-danger">love:</span></p>
<ul>
<li>cat nip</li>
<li>laser pointers</li>
<li>lasagna</li>
</ul>
<p>Top 3 things cats hate:</p>
<ol>
<li>flea treatment</li>
<li>thunder</li>
<li>other cats</li>
</ol>
<form action="/submit-cat-photo">
<div class="row">
<div class="col-xs-6"><label><input type="radio" name="indoor-outdoor"> Indoor</label></div>
<div class="col-xs-6"><label><input type="radio" name="indoor-outdoor"> Outdoor</label></div>
</div>
<label><input type="checkbox" name="personality"> Loving</label>
<label><input type="checkbox" name="personality"> Lazy</label>
<label><input type="checkbox" name="personality"> Crazy</label>
<input type="text" placeholder="cat photo URL" required>
<button type="submit">Submit</button>
</form>
</div>

Responsively Style Checkboxes
你还可以将 Bootstrap 的 col-xs-*用在 form 元素中。这样我们的复选框就可以均匀地在页面上展开了，不管屏幕的分辨率是多大。

将你所有的复选框都放置于一个 <div class="row"> 元素中。然后分别把每个按钮都放置于一个 <div class="col-xs-4"> 元素中。

<link href="//fonts.gdgdocs.org/css?family=Lobster" rel="stylesheet" type="text/css">
<style>
h2 {
font-family: Lobster, Monospace;
}

.thick-green-border {
border-color: green;
border-width: 10px;
border-style: solid;
border-radius: 50%;
}

</style>

<div class="container-fluid">
<div class="row">
<div class="col-xs-8">
<h2 class="text-primary text-center">CatPhotoApp</h2>
</div>
<div class="col-xs-4">
<a href="#">![](/images/relaxing-cat.jpg)</a>
</div>
</div>
![](/images/running-cat.jpg)
<div class="row">
<div class="col-xs-4">
<button class="btn btn-block btn-primary"><i class="fa fa-thumbs-up"></i> Like</button>
</div>
<div class="col-xs-4">
<button class="btn btn-block btn-info"><i class="fa fa-info-circle"></i> Info</button>
</div>
<div class="col-xs-4">
<button class="btn btn-block btn-danger"><i class="fa fa-trash"></i> Delete</button>
</div>
</div>
<p>Things cats <span class="text-danger">love:</span></p>
<ul>
<li>cat nip</li>
<li>laser pointers</li>
<li>lasagna</li>
</ul>
<p>Top 3 things cats hate:</p>
<ol>
<li>flea treatment</li>
<li>thunder</li>
<li>other cats</li>
</ol>
<form action="/submit-cat-photo">
<div class="row">
<div class="col-xs-6">
<label><input type="radio" name="indoor-outdoor"> Indoor</label>
</div>
<div class="col-xs-6">
<label><input type="radio" name="indoor-outdoor"> Outdoor</label>
</div>
</div>
<div class="row">
<div class="col-xs-4"><label><input type="checkbox" name="personality"> Loving</label></div>
<div class="col-xs-4"><label><input type="checkbox" name="personality"> Lazy</label></div>
<div class="col-xs-4"><label><input type="checkbox" name="personality"> Crazy</label></div>
</div>
<input type="text" placeholder="cat photo URL" required>
<button type="submit">Submit</button>
</form>
</div>

Style Text Inputs as Form Controls
你可以在你的 button 提交按钮上添加 Font Awesome的 fa-paper-plane 图标，方法是在元素中增加 <i class="fa fa-paper-plane"></i> 。

给你表单的文本输入框增加 classform-control 。在你的表单提交按钮中增加 class btn btn-primary 。同样，在这个提交按钮中增加 Font Awesome 的 fa-paper-plane 图标。

<link href="//fonts.gdgdocs.org/css?family=Lobster" rel="stylesheet" type="text/css">
<style>
h2 {
font-family: Lobster, Monospace;
}

.thick-green-border {
border-color: green;
border-width: 10px;
border-style: solid;
border-radius: 50%;
}

</style>

<div class="container-fluid">
<div class="row">
<div class="col-xs-8">
<h2 class="text-primary text-center">CatPhotoApp</h2>
</div>
<div class="col-xs-4">
<a href="#">![](/images/relaxing-cat.jpg)</a>
</div>
</div>
![](/images/running-cat.jpg)
<div class="row">
<div class="col-xs-4">
<button class="btn btn-block btn-primary"><i class="fa fa-thumbs-up"></i> Like</button>
</div>
<div class="col-xs-4">
<button class="btn btn-block btn-info"><i class="fa fa-info-circle"></i> Info</button>
</div>
<div class="col-xs-4">
<button class="btn btn-block btn-danger"><i class="fa fa-trash"></i> Delete</button>
</div>
</div>
<p>Things cats <span class="text-danger">love:</span></p>
<ul>
<li>cat nip</li>
<li>laser pointers</li>
<li>lasagna</li>
</ul>
<p>Top 3 things cats hate:</p>
<ol>
<li>flea treatment</li>
<li>thunder</li>
<li>other cats</li>
</ol>
<form action="/submit-cat-photo">
<div class="row">
<div class="col-xs-6">
<label><input type="radio" name="indoor-outdoor"> Indoor</label>
</div>
<div class="col-xs-6">
<label><input type="radio" name="indoor-outdoor"> Outdoor</label>
</div>
</div>
<div class="row">
<div class="col-xs-4">
<label><input type="checkbox" name="personality"> Loving</label>
</div>
<div class="col-xs-4">
<label><input type="checkbox" name="personality"> Lazy</label>
</div>
<div class="col-xs-4">
<label><input type="checkbox" name="personality"> Crazy</label>
</div>
</div>
<input class=form-control type="text" placeholder="cat photo URL" required>
<button class="btn btn-primary" type="submit"><i class="fa fa-paper-plane"></i>Submit</button>
</form>
</div>

Line up Form Elements Responsively with Bootstrap
现在让我们把 input 元素和提交按钮 button 放到同一行。我们将用和之前一样的方法：通过使用拥有 rowclass 属性的 div 元素和其它在它之内的具有 col-xs-*class 属性的 div 元素。

将你的表单中的 input 文本框和提交按钮 button 放到一个具有 row class 属性的 div 元素中。 将你的 input 放置于 class 为 col-xs-7 的 div元素中。 将你的表单的提交按钮 button 放置于 class 属性为 col-xs-5 的 div 元素中。

这是目前为止我们的 Cat Photo 应用的最后一个挑战了。希望你能够喜欢学习 Font Awesome，Bootstrap和响应式设计！

<link href="//fonts.gdgdocs.org/css?family=Lobster" rel="stylesheet" type="text/css">
<style>
h2 {
font-family: Lobster, Monospace;
}

.thick-green-border {
border-color: green;
border-width: 10px;
border-style: solid;
border-radius: 50%;
}

</style>

<div class="container-fluid">
<div class="row">
<div class="col-xs-8">
<h2 class="text-primary text-center">CatPhotoApp</h2>
</div>
<div class="col-xs-4">
<a href="#">![](/images/relaxing-cat.jpg)</a>
</div>
</div>
![](/images/running-cat.jpg)
<div class="row">
<div class="col-xs-4">
<button class="btn btn-block btn-primary"><i class="fa fa-thumbs-up"></i> Like</button>
</div>
<div class="col-xs-4">
<button class="btn btn-block btn-info"><i class="fa fa-info-circle"></i> Info</button>
</div>
<div class="col-xs-4">
<button class="btn btn-block btn-danger"><i class="fa fa-trash"></i> Delete</button>
</div>
</div>
<p>Things cats <span class="text-danger">love:</span></p>
<ul>
<li>cat nip</li>
<li>laser pointers</li>
<li>lasagna</li>
</ul>
<p>Top 3 things cats hate:</p>
<ol>
<li>flea treatment</li>
<li>thunder</li>
<li>other cats</li>
</ol>
<form action="/submit-cat-photo">
<div class="row">
<div class="col-xs-6">
<label><input type="radio" name="indoor-outdoor"> Indoor</label>
</div>
<div class="col-xs-6">
<label><input type="radio" name="indoor-outdoor"> Outdoor</label>
</div>
</div>
<div class="row">
<div class="col-xs-4">
<label><input type="checkbox" name="personality"> Loving</label>
</div>
<div class="col-xs-4">
<label><input type="checkbox" name="personality"> Lazy</label>
</div>
<div class="col-xs-4">
<label><input type="checkbox" name="personality"> Crazy</label>
</div>
</div>
<div class=row>
<div class="col-xs-7"><input type="text" class="form-control" placeholder="cat photo URL" required></div>
<div class="col-xs-5"><button type="submit" class="btn btn-primary"><i class="fa fa-paper-plane"></i> Submit</button></div>
</div>
</form>
</div>

Create a Bootstrap Headline
现在，让我们从头开始练习我们的HTML, CSS 和 Bootstrap 技术。

我们将会搭建一个 jQuery playground，它也即将在我们接下来的 jQuery 课程中被投入使用。

首先，创建一个 h3 元素，并且包含文本内容 jQuery Playground 。

在 h3 元素中设置 Bootstrap 的 class 属性 text-primary 为其上色，同时增加 Bootstrap 的 class 属性 text-center 使文本居中显示。

<h3 class="text-primary text-center">jQuery Playground</h3>
House our page within a Bootstrap Container Fluid Div
现在让我们确保页面里所有的内容都是响应式的。

让我们将 h3 元素放置于一个class属性为 container-fluid的 div 元素中。

<div class="container-fluid">
<h3 class="text-primary text-center">jQuery Playground</h3>
</div>
Create a Bootstrap Row
现在将要为我们的内联元素创建一个 Bootstrap 行。

在 h3 标签下创建一个 div 元素，并且带有 class 属性 row。

<div class="container-fluid">
<h3 class="text-primary text-center">jQuery Playground</h3>
<div class="row"></div>
</div>
Split your Bootstrap Row
既然我们已经有了一个 Bootstrap 行，让我们来把它分成两栏来放置我们的元素吧。

在你的行内添加两个 div 元素，每个都具有 col-xs-6 class 属性。

<div class="container-fluid">
<h3 class="text-primary text-center">jQuery Playground</h3>
<div class="row">
<div class="col-xs-6"></div>
<div class="col-xs-6"></div>
</div>
</div>
Create Bootstrap Wells
Bootstrap 有一个 class 属性叫做 well，它的作用是为设定的列创造出一种视觉上的深度感（一种视觉上的效果，动手写代码体会一下）。

在你的每一个class为col-xs-6的div 元素中都嵌入一个带有 well class 属性的 div 元素。

<div class="container-fluid">
<h3 class="text-primary text-center">jQuery Playground</h3>
<div class="row">
<div class="col-xs-6">
<div class="well"></div>
</div>
<div class="col-xs-6">
<div class="well"></div>
</div>
</div>
</div>
Add Elements within your Bootstrap Wells
现在我们已经在行内的每一列都嵌套了好几层 div 元素了。这已经足够了。现在让我们添加 button 元素吧。

在每一个 well div 元素下放置三个 button 元素。

<div class="container-fluid">
<h3 class="text-primary text-center">jQuery Playground</h3>
<div class="row">
<div class="col-xs-6">
<div class="well">
<button></button>
<button></button>
<button></button>
</div>
</div>
<div class="col-xs-6">
<div class="well">
<button></button>
<button></button>
<button></button>
</div>
</div>
</div>
</div>

Apply the Default Bootstrap Button Style
Bootstrap 还有一种属于按钮的 class 属性叫做 btn-default 。

为你的每一个 button 元素增加两个 class 属性: btn 和 btn-default 。

<div class="container-fluid">
<h3 class="text-primary text-center">jQuery Playground</h3>
<div class="row">
<div class="col-xs-6">
<div class="well">
<button class="btn btn-default"></button>
<button class="btn btn-default"></button>
<button class="btn btn-default"></button>
</div>
</div>
<div class="col-xs-6">
<div class="well">
<button class="btn btn-default"></button>
<button class="btn btn-default"></button>
<button class="btn btn-default"></button>
</div>
</div>
</div>
</div>
Create a Class to Target with jQuery Selectors
并不是每一个 class 属性都是用于 CSS 的。 有些时候我们创建一些 class 只是为了更方便地在jQuery中选中这些元素。

为你的每一个 button 都添加 target class。

<div class="container-fluid">
<h3 class="text-primary text-center">jQuery Playground</h3>
<div class="row">
<div class="col-xs-6">
<div class="well">
<button class="btn btn-default target"></button>
<button class="btn btn-default target"></button>
<button class="btn btn-default target"></button>
</div>
<div class="col-xs-6">
<div class="well">
<button class="btn btn-default target"></button>
<button class="btn btn-default target"></button>
<button class="btn btn-default target"></button>
</div>
</div>
</div>
Add ID Attributes to Bootstrap Elements
回忆一下，我们除了可以给元素增加 class 属性，还可以给你的每个元素增添一个 id 属性。

每一个指定元素的 id 都是唯一的，并且在每个页面中只能使用一次。

现在给我们每个包含 class well 的 div 元素一个唯一的 id。

记住，你可以像这样赋予一个元素 id：

<div class="well" id="center-well">

给左边的 well 赋予 id left-well。给右边的 well 赋予 id right-well。

<div class="container-fluid">
<h3 class="text-primary text-center">jQuery Playground</h3>
<div class="row">
<div class="col-xs-6">
<div class="well" id="left-well">
<button class="btn btn-default target"></button>
<button class="btn btn-default target"></button>
<button class="btn btn-default target"></button>
</div>
</div>
<div class="col-xs-6">
<div class="well" id="right-well">
<button class="btn btn-default target"></button>
<button class="btn btn-default target"></button>
<button class="btn btn-default target"></button>
</div>
</div>
</div>
</div>

Label Bootstrap Wells
让我们为我们的 wells 都标上它们的 id 吧。

在 left-well 之上，class为 col-xs-6 的 div 元素里面，添加一个文本为 #left-well 的 h4元素。

在 right-well 之上，class为 col-xs-6 的 div 元素里面，添加一个文本为 #right-well 的 h4元素。

<div class="container-fluid">
<h3 class="text-primary text-center">jQuery Playground</h3>
<div class="row">
<div class="col-xs-6">
<h4>#left-well</h4>
<div class="well" id="left-well">
<button class="btn btn-default target"></button>
<button class="btn btn-default target"></button>
<button class="btn btn-default target"></button>
</div>
</div>
<div class="col-xs-6">
<h4>#right-well</h4>
<div class="well" id="right-well">
<button class="btn btn-default target"></button>
<button class="btn btn-default target"></button>
<button class="btn btn-default target"></button>
</div>
</div>
</div>
</div>

Give Each Element a Unique ID
我们也可以使用jQuery并通过每个按钮各自唯一的 id 来标识出它们。

给你的每一个按钮一个唯一的 id ，以 target1 为开始，target6 为结束。

确保 target1 到 target3 在 #left-well 之中，target4 到 target6 则在 #right-well 之中。

<div class="container-fluid">
<h3 class="text-primary text-center">jQuery Playground</h3>
<div class="row">
<div class="col-xs-6">
<h4>#left-well</h4>
<div class="well" id="left-well">
<button class="btn btn-default target" id="target1"></button>
<button class="btn btn-default target" id="target2"></button>
<button class="btn btn-default target" id="target3"></button>
</div>
</div>
<div class="col-xs-6">
<h4>#right-well</h4>
<div class="well" id="right-well">
<button class="btn btn-default target" id="target4"></button>
<button class="btn btn-default target" id="target5"></button>
<button class="btn btn-default target" id="target6"></button>
</div>
</div>
</div>
</div>
Label Bootstrap Buttons
正如我们标注了每个 wells， 我们同样想要标注每一个按钮。

为你的每个 button 元素选择与其 id 选择器相同的文本。

<div class="container-fluid">
<h3 class="text-primary text-center">jQuery Playground</h3>
<div class="row">
<div class="col-xs-6">
<h4>#left-well</h4>
<div class="well" id="left-well">
<button class="btn btn-default target" id="target1">#target1</button>
<button class="btn btn-default target" id="target2">#target2</button>
<button class="btn btn-default target" id="target3">#target3</button>
</div>
</div>
<div class="col-xs-6">
<h4>#right-well</h4>
<div class="well" id="right-well">
<button class="btn btn-default target" id="target4">#target4</button>
<button class="btn btn-default target" id="target5">#target5</button>
<button class="btn btn-default target" id="target6">#target6</button>
</div>
</div>
</div>
</div>
Use Comments to Clarify Code
当我们开始使用jQuery，我们将修改HTML元素，但是实际上我们并不是直接在 HTML 文本中修改。

我们必须确保让每个人都知道，他们不应该直接修改此页面上这些代码。

记住，你可以在 为结束的地方进行评论注释。(像这样， )

请在你的 HTML 顶部加如下一段注释：Only change code above this line. 。

<!--Only change code above this line.-->
<div class="container-fluid">
<h3 class="text-primary text-center">jQuery Playground</h3>
<div class="row">
<div class="col-xs-6">
<h4>#left-well</h4>
<div class="well" id="left-well">
<button class="btn btn-default target" id="target1">#target1</button>
<button class="btn btn-default target" id="target2">#target2</button>
<button class="btn btn-default target" id="target3">#target3</button>
</div>
</div>
<div class="col-xs-6">
<h4>#right-well</h4>
<div class="well" id="right-well">
<button class="btn btn-default target" id="target4">#target4</button>
<button class="btn btn-default target" id="target5">#target5</button>
<button class="btn btn-default target" id="target6">#target6</button>
</div>
</div>
</div>
</div>



