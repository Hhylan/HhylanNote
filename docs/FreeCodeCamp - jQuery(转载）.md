FreeCodeCamp - jQuery
（转载）（來源：简书 付林恒 https://www.jianshu.com/p/30e27ca6ad1d）
Learn how Script Tags and Document Ready Work
现在让我们开始学习最流行的JavaScript库jQuery吧，不用担心JavaScript本身，我们稍后会提到它。

在开始学习使用jQuery之前，我们需要加一些代码到HTML文件中。

首先在页面顶端增加一行script元素，然后写上结束符。

浏览器会运行script 里所有的Javascript，包括jQuery。

在你的script里，添加这个方法:$(document).ready(function() {到你的script，接下来用});结束这个方法

接下来我们来学习如何写方法，方法里面的代码会被浏览器加载。

在没有document ready function以前，你的代码会在HTML没有渲染完成就执行，这样会产生bug。

<script>
$(document).ready(function() {});
</script>
<!-- 只更改这条注释以上的代码。 -->

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

Target HTML Elements with Selectors Using jQuery
现在我们已经知道 document ready function的用法了.

现在让我们开始写第一个jQuery语句，所有jQuery方法都是由$开始的，通常称作为 美元符号，或者简称为bling。

jQuery通过选择器来选择一个元素的，然后操作元素做些改变。

举个例子，要让所有的按钮做弹回效果，只要把这段代码写在document ready function里面就可以了。

$("button").addClass("animated bounce");

我们已经在后台为你引入了jQuery库和Animate.css库，这样你就可以在编辑器里直接可以使用这两个库，进而通过jQuery给button元素添加bounce回弹动画效果。

<script>
$(document).ready(function() {
$("button").addClass("animated bounce")
});
</script>

<!-- 只更改这条注释以上的代码。 -->

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

Target Elements by Class Using jQuery
你看到我们是怎么给所有的按钮做弹回效果了吗？我们用 $("button")来选中按钮，然后用.addClass("animated bounce")给按钮加CSS class。

你只需要用jQuery的.addClass()方法，就可以给元素加class了。

首先，我们来使用$(".well")来获取所有class为well的div元素。

仔细想想为什么需要在well前面添加.

然后使用jQuery的.addClass()方法添加2个class：animated、shake。

例如，你可以将下面的代码写在document ready function里：

$(".text-primary").addClass("animated shake");

上面的代码给所有class为text-primary 的元素添加shake class。

<script>
$(document).ready(function() {
$("button").addClass("animated bounce");
$(".well").addClass("animated shake");
});
</script>

<!-- 只更改这条注释以上的代码。 -->

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

Target Elements by ID Using jQuery
你还可以根据id属性来获取元素

首先用$("#target3")来选择id为target3的button元素。

注意，就像CSS一样，在id的名字前加上 #。

然后使用jQuery的.addClass()方法来添加 animated和fadeOutclass.

例如：下面的代码就是给id为target6的button元素添加fade out效果的：

$("#target6").addClass("animated fadeOut")

<script>
$(document).ready(function() {
$("button").addClass("animated bounce");
$(".well").addClass("animated shake");
$("#target3").addClass("fadeOut");
});
</script>

<!-- 只更改这条注释以上的代码。 -->

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

Delete your jQuery Functions
这些动画效果一开始很cool，但是动画太多就有点喧宾夺主了。

在你的document ready function里删掉那三条语句，只留document ready function。

<script>
$(document).ready(function() {

});
</script>

<!-- 只更改这条注释以上的代码。 -->

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
Target the same element with multiple jQuery Selectors
现在你已经了解了3种选择器：元素选择器：$("button")、class选择器：$(".btn")、id选择器：$("#target1")。

尽管用.addClass()这种方式就可以加不同的class，不过还是让我们尝试用不同的方式给元素添加class吧。

用上面介绍的jQuery选择器和addClass()方法：

给所有type为button的元素添加animated class。

给所有class为.btn的按钮添加shake class。

给所有id为#target1的按钮添加btn-primary class。

<script>
$(document).ready(function() {
$("button").addClass("animated");
$(".btn").addClass("shake");
$("#target1").addClass("btn-primary")
});
</script>

<!-- 只更改这条注释以上的代码。 -->

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

Remove classes from an element with jQuery
你可以通过jQuery的addClass()方法给元素添加class,也可以通过jQueryremoveClass()方法去掉元素上的class。

像下面这样：

$("#target2").removeClass("btn-default");

$("#target2").removeClass("btn-default");

来尝试把所有button元素上的btn-default class移除掉。

<script>
$(document).ready(function() {
$("button").addClass("animated bounce");
$(".well").addClass("animated shake");
$("#target3").addClass("animated fadeOut");
$("button").removeClass("btn-default");
});
</script>

<!-- 只更改这条注释以上的代码。 -->

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

Change the CSS of an Element Using jQuery
我们可以通过jQuery来改变HTML元素的CSS样式。

jQuery有一个叫做.css()的方法能让你改变元素的CSS样式。

我们是这样来把颜色改变成蓝色的:

$("#target1").css("color", "blue");

这跟通常的CSS语法有点不同，这里CSS的属性和值是在引号内的，并且用逗号分开。

把你的document ready function清空，

来尝试把target1改变成红色。

<script>
$(document).ready(function() {
$("button").addClass("animated bounce");
$(".well").addClass("animated shake");
$("#target3").addClass("animated fadeOut");
$("button").removeClass("btn-default");
$("#target1").css("color","red");
});
</script>

<!-- 只更改这条注释以上的代码。 -->

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

Disable an Element Using jQuery
你还可以用jQuery改变除了CSS以外的属性。比如，你可以让按钮变不可选。

当你把按钮设置成不可选以后，这会让按钮变灰并且不能点击。

jQuery有一个.prop()的方法让你来调整元素的属性.

我们是这样来让按钮不可选的:

$("button").prop("disabled", true);

$("button").prop("disabled", true);

来尝试让 target1 按钮不可选.

<script>
$(document).ready(function() {
$("#target1").css("color", "red");
$("#target1").prop("disabled", true);
});
</script>

<!-- 只更改这条注释以上的代码。 -->

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

Change Text Inside an Element Using jQuery
jQuery不仅可以改变元素开始标记和结束标记间的文本，甚至可以改变元素标记本身。

jQuery的.html()方法可以添加HTML标签和文字到元素，而元素之前的内容都会被方法的内容所替换掉。

我们是通过em[emphasize]标签来重写和强调标题文本的：

$("h3").html("<em>jQuery Playground</em>");

jQuery 还有一个类似的方法叫.text()，它只能改变文本但不能修改标记。换句话说，这个方法只会把传进来的任何东西(包括标记)当成文本来显示。

任务：强调id为target4按钮里的文本。

<script>
$(document).ready(function() {
$("#target1").css("color", "red");
$("#target4").html("<em>#target4</em>")
});
</script>

<!-- 只更改这条注释以上的代码。 -->

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

Remove an Element Using jQuery
现在让我们用jQuery来移除页面上的HTML元素吧.

jQuery 有一个.remove() 的方法可以移除HTML元素

试着使用.remove()方法来移除页面上的target4元素吧.

<script>
$(document).ready(function() {
$("#target1").css("color", "red");
$("#target1").prop("disabled", true);
$("#target4").remove();
});
</script>

<!-- 只更改这条注释以上的代码。 -->

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

Use appendTo to Move Elements with jQuery
现在让我们尝试把元素从一个div里移到另外一个div里。

jQuery有一个appendTo()方法可以把选中的元素加到其他元素中。

比如，你想让target4从我们的从right-well移到left-well，我们可以这样使用:

$("#target4").appendTo("#left-well");

来试着把target2元素从left-well移到right-well中。

<script>
$(document).ready(function() {
$("#target1").css("color", "red");
$("#target1").prop("disabled", true);
$("#target4").remove();
$("#target2").appendTo("#right-well");
});
</script>

<!-- 只更改这条注释以上的代码。 -->

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

Clone an Element Using jQuery
除了移动元素，你还可以拷贝元素。简单理解：移动元素就是剪切，拷贝元素就是复制。

jQuery的clone()方法可以拷贝元素。

比如，如果我想把target2从left-well拷贝到right-well，我们可以这样写:

$("#target2").clone().appendTo("#right-well");

你有没有发现两个jQuery方法合在一起使用了？这就叫方法链function chaining，使用起来很方便。

复制target5元素追加到left-well。

提示：当你点击run tests后left-well会有两个#target5，千万别以为这是bug。实际上是因为编辑器中的代码会自动执行一次，点击run后会再执行一次，所以有两个#target5。

<script>
$(document).ready(function() {
$("#target1").css("color", "red");
$("#target1").prop("disabled", true);
$("#target4").remove();
$("#target2").appendTo("#right-well");
$("#target5").clone().appendTo("#left-well");
});
</script>

<!-- 只更改这条注释以上的代码。 -->

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

Target the Parent of an Element Using jQuery
每个HTML元素根据继承属性都有父parent元素。

举个例子，h3 元素的父元素是 <div class="container-fluid">，<div class="container-fluid">的父元素是 body。

jQuery有一个方法叫parent()，它允许你访问指定元素的父元素。

举个例子：让left-well 元素的父元素parent()的背景色变成蓝色。

$("#left-well").parent().css("background-color", "blue")

试试让#target1元素的父元素的背景色变成红色。

<script>
$(document).ready(function() {
$("#target1").css("color", "red");
$("#target1").prop("disabled", true);
$("#target4").remove();
$("#target2").appendTo("#right-well");
$("#target5").clone().appendTo("#left-well");
$("#target1").parent().css("background-color","red");
});
</script>

<!-- 只更改这条注释以上的代码。 -->

<body>
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
</body>

Target the Children of an Element Using jQuery
每个人都继承了自己的父母的一些属性，譬如：DNA、相貌、血型、体型等等，HTML也不例外。

许多HTML元素都有children(子元素)，每个子元素都从父元素那里继承了一些属性。

举个例子，每个HTML元素都是 body 的子元素， 你的 "jQuery Playground" h3 元素是 <div class="container-fluid"> 的子元素。

jQuery有一个方法叫children()，它允许你访问指定元素的子元素。

举个例子：让left-well 元素的子元素children()的文本颜色变成蓝色。

$("#left-well").children().css("color", "blue")

任务：让#right-well元素的所有子元素的文本颜色都变成橙色（orange）。

<script>
$(document).ready(function() {
$("#target1").css("color", "red");
$("#target1").prop("disabled", true);
$("#target4").remove();
$("#target2").appendTo("#right-well");
$("#target5").clone().appendTo("#left-well");
$("#target1").parent().css("background-color", "red");
$("#right-well").children().css("color","orange");
});
</script>

<!-- 只更改这条注释以上的代码。 -->

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

Target a Specific Child of an Element Using jQuery
你已经看到了当用jQuery选择器通过id属性来选取元素的时候是多么方便，但是你不能总是写这么整齐的id。

幸运的是，jQuery有一些另外的技巧可以达到同样的效果。

jQuery 用CSS选择器来选取元素，target:nth-child(n)CSS选择器允许你按照索引顺序(从1开始)选择目标元素的所有子元素。

示例：你可以给目标元素的第三个子元素添加bounce class。

$(".target:nth-child(3)").addClass("animated bounce");

任务：确保给目标元素的第二个子元素添加animated和bounce class，你可以通过target class来选获得目标元素。

<script>
$(document).ready(function() {
$("#target1").css("color", "red");
$("#target1").prop("disabled", true);
$("#target4").remove();
$("#target2").appendTo("#right-well");
$("#target5").clone().appendTo("#left-well");
$("#target1").parent().css("background-color", "red");
$("#right-well").children().css("color", "orange");
$(".target:nth-child(2)").addClass("animated bounce");
});
</script>

<!-- 只更改这条注释以上的代码。 -->

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

Target Even Numbered Elements Using jQuery
示例：获取class为target且索引为奇数的所有元素，并给他们添加class。

$(".target:odd").addClass("animated shake");

记住，jQuery里的索引是从0开始的，也就是说：:odd 选择第2、4、6个元素，因为target#2(索引为1)，target#4(索引为3)，target6(索引为5。

任务：获取class为target且索引为偶数的所有元素，也就是target#1(索引为0)，target#3(索引为2)，target5(索引为4)，并给它们添加class animated 和 shake。

<script>
$(document).ready(function() {
$("#target1").css("color", "red");
$("#target1").prop("disabled", true);
$("#target4").remove();
$("#target2").appendTo("#right-well");
$("#target5").clone().appendTo("#left-well");
$("#target1").parent().css("background-color", "red");
$("#right-well").children().css("color", "orange");
$("#left-well").children().css("color", "green");
$(".target:nth-child(2)").addClass("animated bounce");
$(".target:even").addClass("animated shake");
});
</script>

<!-- 只更改这条注释以上的代码。 -->

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

Use jQuery to Modify the Entire Page
我们已经玩了这么久的jQuery游乐场，是时候结束这一节了。

我们让整个body都有淡出效果(fadeOut)： $("body").addClass("animated fadeOut");

让我们做一些更为激动人心的事情，给body添加class animated 和hinge 。

<script>
$(document).ready(function() {
$("#target1").css("color", "red");
$("#target1").prop("disabled", true);
$("#target4").remove();
$("#target2").appendTo("#right-well");
$("#target5").clone().appendTo("#left-well");
$("#target1").parent().css("background-color", "red");
$("#right-well").children().css("color", "orange");
$("#left-well").children().css("color", "green");
$(".target:nth-child(2)").addClass("animated bounce");
$(".target:even").addClass("animated shake");
$("body").addClass("animated hinge");
});
</script>

<!-- 只更改这条注释以上的代码。 -->

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

