FreeCodeCamp - HTML5 and CSS
（转载）（來源：简书 付林恒 https://www.jianshu.com/p/a0b36b32fe6c）
Say Hello to HTML Element
欢迎来到FreeCodeCamp的第一个编码挑战！

整个课程的设计围绕两个原则：所见即所得、循序渐进。

界面简洁直观，左边是课程区、中间是编辑区、右边是显示区。

HTML是英文Hyper Text Markup Language(超文本标记语言)的缩写。

你看到<h1>Hello</h1>了吗?

h1就是一个HTML元素，h1是header1的简写，意思是一级标题。

大部分元素都有一个开始标记和一个结束标记。

开始标记像这样：<h1>

结束标记像这样：</h1>

开始标记和结束标记的唯一区别就是结束标记多了一个/。

每个挑战都有测试，当你写完代码后可以点击Run tests，如果代码通过测试，你将获得学习积分。

如果你点击Run tests后没反应，说明测试没通过，用鼠标拖动课程区的滚动条到最下面，可以看到你没有通过测试的详细原因。

任务：请更改h1标签中的Hello为Hello World，然后点击Run tests。

<h1>Hello World</h1>

Headline with the h2 Element
接下来我们会设计一个类似于下图的页面：


A screen shot of our finished Cat Photo App
h是英文header标题的缩写，标题无处不在，它的应用范围十分广泛：网站结构、写作文、PPT等。h1是主标题，h2是副标题，h3、h4、h5、h6依次递减字体的大小。

在主标题下面创建一个副标题，标题内容是：CatPhotoApp。

<h1>Hello World</h1>
<h2>CatPhotoApp</h2>
Inform with the Paragraph Element
p是英文paragraph段落的缩写，经常被用来创建一个段落，就和你写作文一样。

任务：在副标题下面新增一个段落，段落内容是：Hello Paragraph。

<h1>Hello World</h1>
<h2>我家的猫咪</h2>
<p>hello paragraph</p>
Uncomment HTML
注释有两个功能：

1、想让某一段代码不起作用，但你又不想删除这一段代码。

2、就是给代码添加一些说明，方便团队合作或日后自己查看，但又不想影响代码本身。

我们先学习如何删除注释，再学习如何添加注释。

提示：可以通过删除``来删除注释。

任务：试着先把一级标题、二级标题、段落的注释都删除掉。


<h1>Hello World</h1>

<h2>我家的猫咪</h2>

<p>Hello Paragraph</p>


Comment out HTML
任务：把主标题和段落都注释掉，但把副标题留着。

<!--
<h1>Hello World</h1>
-->
<h2>我家的猫咪</h2>
<!--
<p>Hello Paragraph</p>
-->

Fill in the Blank with Placeholder Text
Web开发者通常用lorem ipsum text来做占位符，占位符就是占着位置的一些文字，没有实际意义。

为什么叫lorem ipsum text呢?

是因为lorem ipsum是古罗马西塞罗谚语的前两个单词。

从公元16世纪开始lorem ipsum text就被当做占位符了，这种传统延续到了互联网时代。

于此同时，孙悟空也在五指山下压了500年，然后就进化成程序猿了，是不是很巧合，哈哈。

任务：把段落中的文本替换为：Monkey code 猴哥猴哥，你真了不得，金箍棒在手，问世间谁是英雄。

<h1>西游记</h1>

<h2>齐天大圣</h2>

<h2>孙悟空</h2>

<p>Monkey code 猴哥猴哥，你真了不得，金箍棒在手，问世间谁是英雄。</p>

Delete HTML Elements
手机的屏幕空间是有限的。

让我们删除不必要的元素，开始设计我们的CatPhotoApp。

任务：删除你的h1元素以简化视图。



<h2>我家的猫咪</h2>

<p>在大家心目中，猫是慵懒的可爱的化身，它可以睡饱了再起来吃饭，可以逗趣小耗子，可以卖得了萌，使得了坏，这样百变的小怪兽就集结在一只宠物上，怎能不惹人怜爱。</p>

Change the Color of Text
现在让我们来改变某些文本的颜色。

我们可以通过修改h2元素的style(样式)来达到目的。

样式的属性有很多，其中color用来指定颜色。

以下是将你的h2元素的文本颜色设置为蓝色的示例代码：

<h2 style="color: blue">CatPhotoApp</h2>

任务：修改你的h2元素的style，让文本的颜色变为红色。

<h2 style="color: red">我家的猫咪</h2>

<p>在大家心目中，猫是慵懒的可爱的化身，它可以睡饱了再起来吃饭，可以逗趣小耗子，可以卖得了萌，使得了坏，这样百变的小怪兽就集结在一只宠物上，怎能不惹人怜爱。</p>

Use CSS Selectors to Style Elements
样式的属性多达几千个，但别担心，按照80-20原则，常用的也就几十个，你完全可以掌握它。

当你键入<h2 style="color: red">CatPhotoApp</h2>，你就给h2元素添加了inline style(内联样式)。

内联样式是为元素添加样式的最简单有效的方式，但是更易于维护的方式是使用层叠样式表CSS（Cascading Style Sheets）。

在代码的最顶端，创建一个如下的style元素：

<style>
</style>

在这个style元素内, 你可以为所有的h2元素创建一个元素选择器。比如，如果你想要将所有的h2元素设置为红色, 你的代码应该看起来像这样：

<style>
选择器 {属性名称: 属性值;}
h2 {color: red;}
</style>

注意：一定要在属性值的后面加上分号;。

任务：删除你的h2元素的内联样式，然后创建一个style元素。添加必要的CSS，使所有h2元素变为蓝色。

<style>
h2 {
color: blue;
}
</style>
<h2>我家的猫咪</h2>

<p>在大家心目中，猫是慵懒的可爱的化身，它可以睡饱了再起来吃饭，可以逗趣小耗子，可以卖得了萌，使得了坏，这样百变的小怪兽就集结在一只宠物上，怎能不惹人怜爱。</p>

Use a CSS Class to Style an Element
上节课我们学习了元素选择器，这节课我们学习类选择器。

我们先声明一个类选择器：

<style>
.blue-text {
​ color: blue;
​ }
​ </style>
​ 
​ 上面的代码在 <style> 标记中声明了一个叫做 blue-text 的类样式。
​ 
​ 然后在h2元素上应用我们声明的类选择器：
​ 
​ <h2 class="blue-text">CatPhotoApp</h2>
​ 
​ 注意：在CSS中，类选择器应该添加.为前缀。
​ 
​ 而在HTML中，class属性不能添加.为前缀。
​ 
​ 这是因为在CSS中如果类选择器前不添加. 浏览器就会误认为类选择器是一个元素选择器。
​ 
​ 任务：在你的style元素中，修改h2选择器为.red-text选择器，并把颜色值从blue修改为red。
​ 
​ 最后在h2元素上应用我们声明的.red-text选择器。
​ 
​ <style>
​ .red-text {
​ color: red;
​ }
​ </style>
​ 
​ <h2 class="red-text">我家的猫咪</h2>
​ 
​ <p>在大家心目中，猫是慵懒的可爱的化身，它可以睡饱了再起来吃饭，可以逗趣小耗子，可以卖得了萌，使得了坏，这样百变的小怪兽就集结在一只宠物上，怎能不惹人怜爱。</p>
​ 
​ Style Multiple Elements with a CSS Class
​ 你可以在 HTML 元素的开始标记中通过使用class="your-class-here"来将 class 附加到相关元素中。
​ 
​ CSS 类选择器必须添加.为前缀，如下：
​ 
​ .blue-text {
​ color: blue;
​ }
​ 
​ 但在HTML中class属性的值不需要添加.为前缀，如下：
​ 
​ <h2 class="blue-text">CatPhotoApp</h2>
​ 
​ 将red-text类应用到h2和p元素中。
​ 
​ <style>
​ .red-text {
​ color: red;
​ }
​ </style>
​ 
​ <h2 class="red-text">我家的猫咪</h2>
​ 
​ <p class="red-text">在大家心目中，猫是慵懒的可爱的化身，它可以睡饱了再起来吃饭，可以逗趣小耗子，可以卖得了萌，使得了坏，这样百变的小怪兽就集结在一只宠物上，怎能不惹人怜爱。</p>
​ 
​ Change the Font Size of an Element
​ 字号是由样式属性font-size来控制的, 如下：
​ 
​ h1 {
​ font-size: 30px;
​ }
​ 
​ 用下面的文本来创建第二个p元素：
​ 养动物有的时候，就是介于爱与恨之间，当你钦羡别人萌宠这么可爱的时候，你一定没有想过，狗狗和猫猫会到处拉屎，甚至会屯老鼠，啃鞋子，用爪子爬门，你不理它，它就挠你，你要对它发脾气，它会比你更来劲。所以，狗猫慎入，没有一定的准备，切勿随便去侍养动物。它们一旦认定你了，你就是它们的主人，如果你抛弃它们，它们必定心中重创。
​ 
​ 任务：让第一个段落和第二个段落的font-size都为16px。
​ 
​ 请不要为第二个段落添加 class 属性。
​ 
​ <style>
​ .red-text {
​ color: red;
​ }
​ p {
​ font-size: 16px;
​ }
​ </style>
​ 
​ <h2 class="red-text">我家的猫咪</h2>
​ 
​ <p class="red-text">在大家心目中，猫是慵懒的可爱的化身，它可以睡饱了再起来吃饭，可以逗趣小耗子，可以卖得了萌，使得了坏，这样百变的小怪兽就集结在一只宠物上，怎能不惹人怜爱。</p>
​ 
​ <p>养动物有的时候，就是介于爱与恨之间，当你钦羡别人萌宠这么可爱的时候，你一定没有想过，狗狗和猫猫会到处拉屎，甚至会屯老鼠，啃鞋子，用爪子爬门，你不理它，它就挠你，你要对它发脾气，它会比你更来劲。所以，狗猫慎入，没有一定的准备，切勿随便去侍养动物。它们一旦认定你了，你就是它们的主人，如果你抛弃它们，它们必定心中重创。</p>
​ Set the Font Family of an Element
​ 用font-family属性来设置元素的字体。
​ 
​ 如果你想把副标题的字体设置为Sans-serif，你可以使用下面的CSS：
​ 
​ h2 {
​ font-family: Sans-serif;
​ }
​ 
​ 任务：让所有的p元素都使用Monospace字体。
​ 
​ <style>
​ .red-text {
​ color: red;
​ }
​ 
​ p {
​ font-size: 16px;
​ font-family: Monospace;
​ }
​ </style>
​ 
​ <h2 class="red-text">CatPhotoApp</h2>
​ 
​ <p class="red-text">在大家心目中，猫是慵懒的可爱的化身，它可以睡饱了再起来吃饭，可以逗趣小耗子，可以卖得了萌，使得了坏，这样百变的小怪兽就集结在一只宠物上，怎能不惹人怜爱。</p>
​ <p>养动物有的时候，就是介于爱与恨之间，当你钦羡别人萌宠这么可爱的时候，你一定没有想过，狗狗和猫猫会到处拉屎，甚至会屯老鼠，啃鞋子，用爪子爬门，你不理它，它就挠你，你要对它发脾气，它会比你更来劲。所以，狗猫慎入，没有一定的准备，切勿随便去侍养动物。它们一旦认定你了，你就是它们的主人，如果你抛弃它们，它们必定心中重创。</p>
​ 
​ Import a Google Font
​ 现在，让我们来导入谷歌字体。
​ 
​ 首先，你需要用link标签来引入谷歌Lobster字体。
​ 
​ 复制下面的代码片断并将其粘贴到你的代码编辑器的顶部：
​ 
​ <link href="https://fonts.gdgdocs.org/css?family=Lobster" rel="stylesheet" type="text/css">
​ 
​ 现在你可以将Lobster作为 font-family属性 的值应用到你的h2元素上了。
​ 
​ 为你的h2元素应用font-family属性，值为Lobster。
​ 
​ 当你遇到困难时可以参考wiki
​ 
​ <link href="https://fonts.gdgdocs.org/css?family=Lobster" rel="stylesheet" type="text/css">
​ <style>
​ .red-text {
​ color: red;
​ }
​ 
​ p {
​ font-size: 16px;
​ font-family: Monospace;
​ }
​ 
​ h2 {
​ font-family: Lobster;
​ }
​ </style>
​ 
​ <h2 class="red-text">CatPhotoApp</h2>
​ 
​ <p class="red-text">在大家心目中，猫是慵懒的可爱的化身，它可以睡饱了再起来吃饭，可以逗趣小耗子，可以卖得了萌，使得了坏，这样百变的小怪兽就集结在一只宠物上，怎能不惹人怜爱。</p>
​ <p class="red-text">养动物有的时候，就是介于爱与恨之间，当你钦羡别人萌宠这么可爱的时候，你一定没有想过，狗狗和猫猫会到处拉屎，甚至会屯老鼠，啃鞋子，用爪子爬门，你不理它，它就挠你，你要对它发脾气，它会比你更来劲。所以，狗猫慎入，没有一定的准备，切勿随便去侍养动物。它们一旦认定你了，你就是它们的主人，如果你抛弃它们，它们必定心中重创。</p>
​ 
​ Specify How Fonts Should Degrade
​ 有几种默认的字体是所有浏览器都可用的，包括Monospace、Serif和Sans-Serif。
​ 
​ 当某种字体不可用时，你可以让浏览器自动降级到另一种字体。
​ 
​ 例如，如果你想让段落的字体为Helvetica，但你同时想在Helvetica字体不可用时自动降级使用Sans-Serif字体，你可以使用如下CSS样式：
​ 
​ p {
​ font-family: Helvetica, Sans-Serif;
​ }
​ 
​ 现在注释掉link标签，以使Lobster字体不可用。请仔细观察浏览器是如何降级到Monospace字体的。
​ 
​ <!--<link href="https://fonts.gdgdocs.org/css?family=Lobster" rel="stylesheet" type="text/css">-->
​ <style>
​ .red-text {
​ color: red;
​ }
​ 
​ h2 {
​ font-family: Lobster, Monospace;
​ }
​ 
​ p {
​ font-size: 16px;
​ font-family: Monospace;
​ }
​ </style>
​ 
​ <h2 class="red-text">CatPhotoApp</h2>
​ 
​ <p class="red-text">在大家心目中，猫是慵懒的可爱的化身，它可以睡饱了再起来吃饭，可以逗趣小耗子，可以卖得了萌，使得了坏，这样百变的小怪兽就集结在一只宠物上，怎能不惹人怜爱。</p>
​ <p class="red-text">养动物有的时候，就是介于爱与恨之间，当你钦羡别人萌宠这么可爱的时候，你一定没有想过，狗狗和猫猫会到处拉屎，甚至会屯老鼠，啃鞋子，用爪子爬门，你不理它，它就挠你，你要对它发脾气，它会比你更来劲。所以，狗猫慎入，没有一定的准备，切勿随便去侍养动物。它们一旦认定你了，你就是它们的主人，如果你抛弃它们，它们必定心中重创。</p>
​ 
​ Add Images to your Website
​ 使用img元素来为你的网站添加图片，使用src属性指向一个图片的具体地址。
​ 
​ 举例如下：
​ 
​ [图片上传失败...(image-791300-1510046527278)]
​ 
​ 注意：img元素是自关闭元素，不需要结束标记。
​ 
​ 用以下图片来测试：
​ 
​ /images/relaxing-cat.jpg
​ 
​ <link href="https://fonts.gdgdocs.org/css?family=Lobster" rel="stylesheet" type="text/css">
​ <style>
​ .red-text {
​ color: red;
​ }
​ 
​ h2 {
​ font-family: Lobster, Monospace;
​ }
​ 
​ p {
​ font-size: 16px;
​ font-family: Monospace;
​ }
​ </style>
​ 
​ <h2 class="red-text">我家的猫咪</h2>
​ ![](/images/relaxing-cat.jpg)
​ <p class="red-text">猫咪猫咪我就喜欢你</p>
​ <p class="red-text">深深地爱上你</p>
​ <p class="red-text">没有理由没有原因</p>
​ <p class="red-text">从见到你的那一天起</p>
​ <p class="red-text">你知道我在等你吗?</p>
​ <p class="red-text">你如果真的在乎我</p>
​ <p class="red-text">又怎会让无尽的夜陪我度过</p>
​ <p class="red-text">猫咪猫咪我就喜欢你</p>
​ <p class="red-text">深深地爱上你</p>
​ <p class="red-text">在黑夜里倾听你的声音</p>
​ 
​ Size your Images
​ CSS包含一个控制元素宽度的width属性。像控制字体一样，我们使用px（像素）来指定图片的宽度。
​ 
​ 例如，如果我们想要创建一个名为larger-image的类选择器，把HTML元素的宽度设定为500像素，我们使用：
​ 
​ <style>
​ .larger-image {
​ width: 500px;
​ }
​ </style>
​ 
​ 任务：创建一个名为smaller-image的类选择器，然后用它来改变图片尺寸，使图片仅有100像素宽。
​ 
​ <link href="https://fonts.gdgdocs.org/css?family=Lobster" rel="stylesheet" type="text/css">
​ <style>
​ .red-text {
​ color: red;
​ }
​ 
​ h2 {
​ font-family: Lobster, Monospace;
​ }
​ 
​ p {
​ font-size: 16px;
​ font-family: Monospace;
​ }
​ 
​ .smaller-image {
​ width: 100px;
​ }
​ </style>
​ 
​ <h2 class="red-text">CatPhotoApp</h2>
​ 
​ ![](/images/relaxing-cat.jpg)
​ 
​ <p class="red-text">在大家心目中，猫是慵懒的可爱的化身，它可以睡饱了再起来吃饭，可以逗趣小耗子，可以卖得了萌，使得了坏，这样百变的小怪兽就集结在一只宠物上，怎能不惹人怜爱。</p>
​ <p class="red-text">养动物有的时候，就是介于爱与恨之间，当你钦羡别人萌宠这么可爱的时候，你一定没有想过，狗狗和猫猫会到处拉屎，甚至会屯老鼠，啃鞋子，用爪子爬门，你不理它，它就挠你，你要对它发脾气，它会比你更来劲。所以，狗猫慎入，没有一定的准备，切勿随便去侍养动物。它们一旦认定你了，你就是它们的主人，如果你抛弃它们，它们必定心中重创。</p>
​ 
​ Add Borders Around your Elements
​ CSS 边框的属性有style(样式)、color(颜色)、width(宽度)、height(高度)等。
​ 
​ 举个例子，如果我们想要让一个HTML元素的边框颜色为红色、边框宽度为5像素(px)、边框样式为固体(solid)，代码如下:
​ 
​ <style>
​ .thin-red-border {
​ border-color: red;
​ border-width: 5px;
​ border-style: solid;
​ }
​ </style>
​ 
​ 任务：创建一个叫thick-green-border的class，让它的边框宽度为10像素、边框样式为solid(固体)、边框颜色为绿色(green)，然后把这个class应用到你的猫咪照片上。
​ 
​ 提示：你可以应用多个class到一个元素，只需要在多个class之间用空格分开即可。例如：
​ 
​ <img class="class1 class2">
​ 
​ <link href="https://fonts.gdgdocs.org/css?family=Lobster" rel="stylesheet" type="text/css">
​ <style>
​ .red-text {
​ color: red;
​ }
​ 
​ h2 {
​ font-family: Lobster, Monospace;
​ }
​ 
​ p {
​ font-size: 16px;
​ font-family: Monospace;
​ }
​ 
​ .smaller-image {
​ width: 100px;
​ }
​ 
​ .thick-green-border {
​ border-color: green;
​ border-width: 10px;
​ border-style: solid;
​ }
​ </style>
​ 
​ <h2 class="red-text">CatPhotoApp</h2>
​ 
​ ![](/images/relaxing-cat.jpg)
​ 
​ <p class="red-text">在大家心目中，猫是慵懒的可爱的化身，它可以睡饱了再起来吃饭，可以逗趣小耗子，可以卖得了萌，使得了坏，这样百变的小怪兽就集结在一只宠物上，怎能不惹人怜爱。</p>
​ <p class="red-text">养动物有的时候，就是介于爱与恨之间，当你钦羡别人萌宠这么可爱的时候，你一定没有想过，狗狗和猫猫会到处拉屎，甚至会屯老鼠，啃鞋子，用爪子爬门，你不理它，它就挠你，你要对它发脾气，它会比你更来劲。所以，狗猫慎入，没有一定的准备，切勿随便去侍养动物。它们一旦认定你了，你就是它们的主人，如果你抛弃它们，它们必定心中重创。</p>
​ 
​ Add Rounded Corners with a Border Radius
​ 猫咪图片的边框现在是尖尖的，不够可爱，我们可以通过CSS的一个叫border-radius(边框半径)的属性来让它的边框变成圆的。
​ 
​ 你同样可以使用像素来指定border-radius的属性值，现在让你的猫咪图片的边框半径为10px吧。
​ 
​ 注意：这个任务有多种解决方案。你可以添加border-radius到.thick-green-border类选择器，也可以添加到.smaller-image类选择器.
​ 
​ <link href="https://fonts.gdgdocs.org/css?family=Lobster" rel="stylesheet" type="text/css">
​ <style>
​ .red-text {
​ color: red;
​ }
​ 
​ h2 {
​ font-family: Lobster, Monospace;
​ }
​ 
​ p {
​ font-size: 16px;
​ font-family: Monospace;
​ }
​ 
​ .thick-green-border {
​ border-color: green;
​ border-width: 10px;
​ border-style: solid;
​ border-radius: 10px;
​ }
​ 
​ .smaller-image {
​ width: 100px;
​ }
​ </style>
​ 
​ <h2 class="red-text">我家的猫咪</h2>
​ 
​ ![](/images/relaxing-cat.jpg)
​ 
​ <p class="red-text">我家两岁的小公猫哈哈是个收藏家，臭鱼烂虾，鸡头猪手，无所不爱。清晨我还在睡梦中，突然觉得胸口一沉，恍惚中意识到哈哈又跑到我身上来撒娇，心里不由得滚起温暖的热流，拉过哈哈一把从头摸过背，小家伙顺势想往被子里钻，我一边拒绝着一边往上拉被子，突然脚下一凉，烂泥一样挂在我的大脚趾上的是一块垃圾箱里的鱼头！我顿时睡意全无，换床单洗被罩，天光放亮才勉强收拾妥当。害得我带着熊猫眼跑去上班，一天都没有好心情。实在搞不懂它为什么爱把垃圾叼上床，是故意恶作剧？还是我给的猫粮不够吃？</p>
​ <p class="red-text">有时候猫会把主人当成自己的孩子(听起来有点令人窝心)，这种行为是在给家里带来猎物。它把自己看成是家里的顶梁柱，有责任给不争气的主人找来食物——猫咪通过长时间对你的观察，沉痛地发现你不会打猎。经常出门的猫咪会把它逮到的老鼠、小鸟带回家里，不出门的就经常翻翻垃圾箱找点东西给你。这个时候，主人可不要责骂它，不然它会认为你对它带回来的食物不满意，下次去找更了不起的东西带回来，放在房间里最显眼的地方。但如果你看见它往家里运输死老鼠，最好也别谢它，别让它觉得你对这种猎物很满意，下次照单带回来。最好的办法是心里感念着猫咪所为你做的，并默默地收拾好一切。</p>
​ 
​ Make Circular Images with a Border Radius
​ 除了像素，你还可以使用百分比来指定border-radius边框半径的值。
​ 
​ 给你的猫咪图片一个50%的border-radius。
​ 
​ <link href="https://fonts.gdgdocs.org/css?family=Lobster" rel="stylesheet" type="text/css">
​ <style>
​ .red-text {
​ color: red;
​ }
​ 
​ h2 {
​ font-family: Lobster, Monospace;
​ }
​ 
​ p {
​ font-size: 16px;
​ font-family: Monospace;
​ }
​ 
​ .thick-green-border {
​ border-color: green;
​ border-width: 10px;
​ border-style: solid;
​ border-radius: 50%;
​ }
​ 
​ .smaller-image {
​ width: 100px;
​ }
​ </style>
​ 
​ <h2 class="red-text">CatPhotoApp</h2>
​ 
​ ![](/images/relaxing-cat.jpg)
​ 
​ <p class="red-text">在大家心目中，猫是慵懒的可爱的化身，它可以睡饱了再起来吃饭，可以逗趣小耗子，可以卖得了萌，使得了坏，这样百变的小怪兽就集结在一只宠物上，怎能不惹人怜爱。</p>
​ <p class="red-text">养动物有的时候，就是介于爱与恨之间，当你钦羡别人萌宠这么可爱的时候，你一定没有想过，狗狗和猫猫会到处拉屎，甚至会屯老鼠，啃鞋子，用爪子爬门，你不理它，它就挠你，你要对它发脾气，它会比你更来劲。所以，狗猫慎入，没有一定的准备，切勿随便去侍养动物。它们一旦认定你了，你就是它们的主人，如果你抛弃它们，它们必定心中重创。</p>
​ 
​ Link to External Pages with Anchor Elements
​ a元素，也叫anchor（锚点）元素，既可以用来链接到外部地址实现页面跳转功能，也可以链接到当前页面的某部分实现内部导航功能。
​ 
​ 下面是一张a元素的图示。a元素位于段落元素的中间，这意味着链接会出现在段落的中间。
​ 
​ 
​ a diagram of how anchor tags are composed with the same text as on the following line
​ 这有一个例子：
​ 
​ <p>Here's a <a href="http://freecodecamp.cn"> link to FreeCodeCamp中文社区 </a> for you to follow.</p>
​ 
​ 任务：创建一个链接到http://freecatphotoapp.com的a元素，并用cat photos作为其anchor text（锚点文本）。
​ 
​ <link href="https://fonts.gdgdocs.org/css?family=Lobster" rel="stylesheet" type="text/css">
​ <style>
​ .red-text {
​ color: red;
​ }
​ 
​ h2 {
​ font-family: Lobster, Monospace;
​ }
​ 
​ p {
​ font-size: 16px;
​ font-family: Monospace;
​ }
​ 
​ .thick-green-border {
​ border-color: green;
​ border-width: 10px;
​ border-style: solid;
​ border-radius: 50%;
​ }
​ 
​ .smaller-image {
​ width: 100px;
​ }
​ </style>
​ <a href="http://freecatphotoapp.com">cat photos</a>
​ <h2 class="red-text">CatPhotoApp</h2>
​ 
​ ![](/images/relaxing-cat.jpg)
​ 
​ <p class="red-text">在大家心目中，猫是慵懒的可爱的化身，它可以睡饱了再起来吃饭，可以逗趣小耗子，可以卖得了萌，使得了坏，这样百变的小怪兽就集结在一只宠物上，怎能不惹人怜爱。</p>
​ <p class="red-text">养动物有的时候，就是介于爱与恨之间，当你钦羡别人萌宠这么可爱的时候，你一定没有想过，狗狗和猫猫会到处拉屎，甚至会屯老鼠，啃鞋子，用爪子爬门，你不理它，它就挠你，你要对它发脾气，它会比你更来劲。所以，狗猫慎入，没有一定的准备，切勿随便去侍养动物。它们一旦认定你了，你就是它们的主人，如果你抛弃它们，它们必定心中重创。</p>
​ 
​ Nest an Anchor Element within a Paragraph
​ 作为参考，再次看一看a元素的图示：
​ 
​ 
​ a diagram of how anchor tags are composed with the same text as on the following line
​ 例如：
​ 
​ <p>Here's a <a href="https://freecodecamp.cn"> link to FreeCodeCamp中文社区</a> for you to follow.</p>
​ 
​ Nesting（嵌套）就是把一个元素放在另一个元素里面。
​ 
​ 任务：把你的a元素嵌套进一个新的p元素（紧邻已有的h2元素之后），让段落的文本为View more cat photos，但是其中仅cat photos是一个链接，其余的是普通文本。
​ 
​ <link href="https://fonts.gdgdocs.org/css?family=Lobster" rel="stylesheet" type="text/css">
​ <style>
​ .red-text {
​ color: red;
​ }
​ 
​ h2 {
​ font-family: Lobster, Monospace;
​ }
​ 
​ p {
​ font-size: 16px;
​ font-family: Monospace;
​ }
​ 
​ .thick-green-border {
​ border-color: green;
​ border-width: 10px;
​ border-style: solid;
​ border-radius: 50%;
​ }
​ 
​ .smaller-image {
​ width: 100px;
​ }
​ </style>
​ 
​ <h2 class="red-text">CatPhotoApp</h2>
​ <!-- 只更改这条注释以下的代码。 -->
​ 
​ <p>View more <a href="http://www.freecatphotoapp.com">cat photos</a></p>
​ 
​ <!-- 只更改这条注释以上的代码。 -->
​ ![](/images/relaxing-cat.jpg)
​ 
​ <p class="red-text">在大家心目中，猫是慵懒的可爱的化身，它可以睡饱了再起来吃饭，可以逗趣小耗子，可以卖得了萌，使得了坏，这样百变的小怪兽就集结在一只宠物上，怎能不惹人怜爱。</p>
​ <p class="red-text">养动物有的时候，就是介于爱与恨之间，当你钦羡别人萌宠这么可爱的时候，你一定没有想过，狗狗和猫猫会到处拉屎，甚至会屯老鼠，啃鞋子，用爪子爬门，你不理它，它就挠你，你要对它发脾气，它会比你更来劲。所以，狗猫慎入，没有一定的准备，切勿随便去侍养动物。它们一旦认定你了，你就是它们的主人，如果你抛弃它们，它们必定心中重创。</p>
​ 
​ Make Dead Links using the Hash Symbol
​ 有时你想为你的网站添加一个a元素，但此时你还不知道要将它们链接到哪儿，此时可以使用固定链接。
​ 
​ 把你的a元素的href属性的值替换为一个#，别名hash(哈希)符号，将其变为一个固定链接。
​ 
​ <link href="https://fonts.gdgdocs.org/css?family=Lobster" rel="stylesheet" type="text/css">
​ <style>
​ .red-text {
​ color: red;
​ }
​ 
​ h2 {
​ font-family: Lobster, Monospace;
​ }
​ 
​ p {
​ font-size: 16px;
​ font-family: Monospace;
​ }
​ 
​ .thick-green-border {
​ border-color: green;
​ border-width: 10px;
​ border-style: solid;
​ border-radius: 50%;
​ }
​ 
​ .smaller-image {
​ width: 100px;
​ }
​ </style>
​ 
​ <h2 class="red-text">CatPhotoApp</h2>
​ 
​ <p>Click here for <a href="#">cat photos</a>.</p>
​ 
​ ![](/images/relaxing-cat.jpg)
​ 
​ <p class="red-text">在大家心目中，猫是慵懒的可爱的化身，它可以睡饱了再起来吃饭，可以逗趣小耗子，可以卖得了萌，使得了坏，这样百变的小怪兽就集结在一只宠物上，怎能不惹人怜爱。</p>
​ <p class="red-text">养动物有的时候，就是介于爱与恨之间，当你钦羡别人萌宠这么可爱的时候，你一定没有想过，狗狗和猫猫会到处拉屎，甚至会屯老鼠，啃鞋子，用爪子爬门，你不理它，它就挠你，你要对它发脾气，它会比你更来劲。所以，狗猫慎入，没有一定的准备，切勿随便去侍养动物。它们一旦认定你了，你就是它们的主人，如果你抛弃它们，它们必定心中重创。</p>
​ 
​ Turn an Image into a Link
​ 你可以通过把某元素嵌套进a元素使其变成一个链接。
​ 
​ 把你的图片嵌套进a元素。举例如下：
​ 
​ <a href="#">[图片上传失败...(image-65ea48-1510046527278)]</a>
​ 
​ 任务：把你的小猫图片插入到一个新的锚点元素中，并把锚点元素的href属性设置为#。
​ 
​ 一旦完成，把你的光标悬停在你的图片上。你的光标此时应该由光标指针变成手形指针。图片现在是一个链接了。
​ 
​ <link href="https://fonts.gdgdocs.org/css?family=Lobster" rel="stylesheet" type="text/css">
​ <style>
​ .red-text {
​ color: red;
​ }
​ 
​ h2 {
​ font-family: Lobster, Monospace;
​ }
​ 
​ p {
​ font-size: 16px;
​ font-family: Monospace;
​ }
​ 
​ .thick-green-border {
​ border-color: green;
​ border-width: 10px;
​ border-style: solid;
​ border-radius: 50%;
​ }
​ 
​ .smaller-image {
​ width: 100px;
​ }
​ </style>
​ 
​ <h2 class="red-text">CatPhotoApp</h2>
​ 
​ <p>Click here for <a href="#">cat photos</a>.</p>
​ 
​ <a href="#">![](/images/relaxing-cat.jpg)</a>
​ 
​ <p class="red-text">在大家心目中，猫是慵懒的可爱的化身，它可以睡饱了再起来吃饭，可以逗趣小耗子，可以卖得了萌，使得了坏，这样百变的小怪兽就集结在一只宠物上，怎能不惹人怜爱。</p>
​ <p class="red-text">养动物有的时候，就是介于爱与恨之间，当你钦羡别人萌宠这么可爱的时候，你一定没有想过，狗狗和猫猫会到处拉屎，甚至会屯老鼠，啃鞋子，用爪子爬门，你不理它，它就挠你，你要对它发脾气，它会比你更来劲。所以，狗猫慎入，没有一定的准备，切勿随便去侍养动物。它们一旦认定你了，你就是它们的主人，如果你抛弃它们，它们必定心中重创。</p>
​ 
​ Add Alt Text to an Image for Accessibility
​ alt属性，也被称为alt text, 是当图片无法加载时显示的替代文本。alt属性对于盲人或视觉损伤的用户理解一幅图片中所描绘的内容非常重要，搜索引擎也会搜索alt属性。
​ 
​ 简而言之，每一张图片都应该有一个alt属性！
​ 
​ 你可以像下面例子中一样为img元素添加一个alt属性：
​ 
​ [图片上传失败...(image-4bb944-1510046527278)]
​ 
​ 为你的猫咪图片添加一个alt属性，内容为A cute orange cat lying on its back。
​ 
​ <link href="https://fonts.gdgdocs.org/css?family=Lobster" rel="stylesheet" type="text/css">
​ <style>
​ .red-text {
​ color: red;
​ }
​ 
​ h2 {
​ font-family: Lobster, Monospace;
​ }
​ 
​ p {
​ font-size: 16px;
​ font-family: Monospace;
​ }
​ 
​ .thick-green-border {
​ border-color: green;
​ border-width: 10px;
​ border-style: solid;
​ border-radius: 50%;
​ }
​ 
​ .smaller-image {
​ width: 100px;
​ }
​ </style>
​ 
​ <h2 class="red-text">CatPhotoApp</h2>
​ 
​ <p>Click here for <a href="#">cat photos</a>.</p>
​ 
​ <a href="#">![](/images/relaxing-cat.jpg)</a>
​ 
​ <p class="red-text">在大家心目中，猫是慵懒的可爱的化身，它可以睡饱了再起来吃饭，可以逗趣小耗子，可以卖得了萌，使得了坏，这样百变的小怪兽就集结在一只宠物上，怎能不惹人怜爱。</p>
​ <p class="red-text">养动物有的时候，就是介于爱与恨之间，当你钦羡别人萌宠这么可爱的时候，你一定没有想过，狗狗和猫猫会到处拉屎，甚至会屯老鼠，啃鞋子，用爪子爬门，你不理它，它就挠你，你要对它发脾气，它会比你更来劲。所以，狗猫慎入，没有一定的准备，切勿随便去侍养动物。它们一旦认定你了，你就是它们的主人，如果你抛弃它们，它们必定心中重创。</p>
​ 
​ Create a Bulleted Unordered List
​ HTML有一个特殊元素，用于创建unordered lists（无序列表）, 或带项目符号的列表。
​ 
​ 无序列表以<ul>元素开始，并包含一个或多个<li>元素。
​ 
​ 例如：
​ 
​ <ul>
​ <li>milk</li>
​ <li>cheese</li>
​ </ul>
​ 
​ 将会创建一个带项目符号的"milk"和"cheese"列表。
​ 
​ 删除最后两个p元素，然后在页面底部创建一个有关猫咪喜欢的三件事情的无序列表。
​ 
​ <link href="https://fonts.gdgdocs.org/css?family=Lobster" rel="stylesheet" type="text/css">
​ <style>
​ .red-text {
​ color: red;
​ }
​ 
​ h2 {
​ font-family: Lobster, Monospace;
​ }
​ 
​ p {
​ font-size: 16px;
​ font-family: Monospace;
​ }
​ 
​ .thick-green-border {
​ border-color: green;
​ border-width: 10px;
​ border-style: solid;
​ border-radius: 50%;
​ }
​ 
​ .smaller-image {
​ width: 100px;
​ }
​ </style>
​ 
​ <h2 class="red-text">CatPhotoApp</h2>
​ 
​ <p>Click here for <a href="#">cat photos</a>.</p>
​ 
​ <a href="#">![](/images/relaxing-cat.jpg)</a>
​ 
​ <ul>
​ <li>吃饭</li>
​ <li>睡觉</li>
​ <li>抓老鼠</li>
​ </ul>
​ Create an Ordered List
​ HTML有一个特殊元素，用于创建ordered lists（有序列表）, 或数字编号列表。
​ 
​ 有序列表以<ol>元素开始，并包含一个或多个<li>元素。
​ 
​ 例如：
​ 
​ <ol>
​ <li>Garfield</li>
​ <li>Sylvester</li>
​ </ol>
​ 
​ 将创建一个包含"Garfield"和"Sylvester"的数字编号列表。
​ 
​ 创建一个有关猫咪最痛恨的三件事情Top 3 things cats hate:的有序列表。
​ 
​ <link href="https://fonts.gdgdocs.org/css?family=Lobster" rel="stylesheet" type="text/css">
​ <style>
​ .red-text {
​ color: red;
​ }
​ 
​ h2 {
​ font-family: Lobster, Monospace;
​ }
​ 
​ p {
​ font-size: 16px;
​ font-family: Monospace;
​ }
​ 
​ .thick-green-border {
​ border-color: green;
​ border-width: 10px;
​ border-style: solid;
​ border-radius: 50%;
​ }
​ 
​ .smaller-image {
​ width: 100px;
​ }
​ </style>
​ 
​ <h2 class="red-text">CatPhotoApp</h2>
​ 
​ <p>Click here for <a href="#">cat photos</a>.</p>
​ 
​ <a href="#">![](/images/relaxing-cat.jpg)</a>
​ 
​ <p>Things cats love:</p>
​ <ul>
​ <li>cat nip</li>
​ <li>laser pointers</li>
​ <li>lasagna</li>
​ </ul>
​ <p>Top 3 things cats hate:</p>
​ <!-- 请只更改下方HTML来避免错误 -->
​ <ol>
​ <li>cat nip</li>
​ <li>laser pointers</li>
​ <li>lasagna</li>
​ </ol>
​ Create a Text Field
​ 现在让我们来创建一个form(表单)。
​ 
​ Text input(文本输入框)是用来获得用户输入的绝佳方式。
​ 
​ 你可以用如下方法创建：
​ 
​ <input type="text">
​ 
​ 注意，input元素是自关闭的。
​ 
​ 任务：在有序列表下面创建一个type(类型)为text的input元素。
​ 
​ <link href="https://fonts.gdgdocs.org/css?family=Lobster" rel="stylesheet" type="text/css">
​ <style>
​ .red-text {
​ color: red;
​ }
​ 
​ h2 {
​ font-family: Lobster, Monospace;
​ }
​ 
​ p {
​ font-size: 16px;
​ font-family: Monospace;
​ }
​ 
​ .thick-green-border {
​ border-color: green;
​ border-width: 10px;
​ border-style: solid;
​ border-radius: 50%;
​ }
​ 
​ .smaller-image {
​ width: 100px;
​ }
​ </style>
​ 
​ <h2 class="red-text">CatPhotoApp</h2>
​ 
​ <p>Click here for <a href="#">cat photos</a>.</p>
​ 
​ <a href="#">![](/images/relaxing-cat.jpg)</a>
​ 
​ <p>Things cats love:</p>
​ <ul>
​ <li>cat nip</li>
​ <li>laser pointers</li>
​ <li>lasagna</li>
​ </ul>
​ <p>Top 3 things cats hate:</p>
​ <ol>
​ <li>flea treatment</li>
​ <li>thunder</li>
​ <li>other cats</li>
​ </ol>
​ <input type="text">
​ Add Placeholder Text to a Text Field
​ 占位符(placeholder text)是用户在input(输入)框输入任何东西之前放置在input(输入)框中的预定义文本。
​ 
​ 你可以用如下方式创建占位符：
​ 
​ <input type="text" placeholder="this is placeholder text">
​ 
​ 把你的input(输入)框的placeholder的值设置为"cat photo URL"。
​ 
​ <link href="https://fonts.gdgdocs.org/css?family=Lobster" rel="stylesheet" type="text/css">
​ <style>
​ .red-text {
​ color: red;
​ }
​ 
​ h2 {
​ font-family: Lobster, Monospace;
​ }
​ 
​ p {
​ font-size: 16px;
​ font-family: Monospace;
​ }
​ 
​ .thick-green-border {
​ border-color: green;
​ border-width: 10px;
​ border-style: solid;
​ border-radius: 50%;
​ }
​ 
​ .smaller-image {
​ width: 100px;
​ }
​ </style>
​ 
​ <h2 class="red-text">CatPhotoApp</h2>
​ 
​ <p>Click here for <a href="#">cat photos</a>.</p>
​ 
​ <a href="#">![](/images/relaxing-cat.jpg)</a>
​ 
​ <p>Things cats love:</p>
​ <ul>
​ <li>cat nip</li>
​ <li>laser pointers</li>
​ <li>lasagna</li>
​ </ul>
​ <p>Top 3 things cats hate:</p>
​ <ol>
​ <li>flea treatment</li>
​ <li>thunder</li>
​ <li>other cats</li>
​ </ol>
​ <input type="text" placeholder="cat photo URL">
​ 
​ Create a Form Element
​ 使用HTML来构建可以跟服务器交互的Web表单(form)，通过给你的form元素添加一个action属性来达到此目的。
​ 
​ action属性的值指定了表单提交到服务器的地址。
​ 
​ 例如：
​ 
​ <form action="/url-where-you-want-to-submit-form-data"></form>
​ 
​ 把你的文本框嵌套进form元素，并为此form元素添加action="/submit-cat-photo"。
​ 
​ <link href="https://fonts.gdgdocs.org/css?family=Lobster" rel="stylesheet" type="text/css">
​ <style>
​ .red-text {
​ color: red;
​ }
​ 
​ h2 {
​ font-family: Lobster, Monospace;
​ }
​ 
​ p {
​ font-size: 16px;
​ font-family: Monospace;
​ }
​ 
​ .thick-green-border {
​ border-color: green;
​ border-width: 10px;
​ border-style: solid;
​ border-radius: 50%;
​ }
​ 
​ .smaller-image {
​ width: 100px;
​ }
​ </style>
​ 
​ <h2 class="red-text">CatPhotoApp</h2>
​ 
​ <p>Click here for <a href="#">cat photos</a>.</p>
​ 
​ <a href="#">![](/images/relaxing-cat.jpg)</a>
​ 
​ <p>Things cats love:</p>
​ <ul>
​ <li>cat nip</li>
​ <li>laser pointers</li>
​ <li>lasagna</li>
​ </ul>
​ <p>Top 3 things cats hate:</p>
​ <ol>
​ <li>flea treatment</li>
​ <li>thunder</li>
​ <li>other cats</li>
​ </ol>
​ <form action="/submit-cat-photo"><input type="text" placeholder="cat photo URL"></form>
​ 
​ Add a Submit Button to a Form
​ 让我们来为你的form添加一个submit(提交)按钮，点击这个按钮，表单中的数据将会被发送到你通过action属性指定的地址上。
​ 
​ 下面是submit按钮的例子：
​ 
​ <button type="submit">this button submits the form</button>
​ 
​ 为你的form元素添加一个type为submit的提交按钮，用"Submit"作按钮文本。
​ 
​ <link href="https://fonts.gdgdocs.org/css?family=Lobster" rel="stylesheet" type="text/css">
​ <style>
​ .red-text {
​ color: red;
​ }
​ 
​ h2 {
​ font-family: Lobster, Monospace;
​ }
​ 
​ p {
​ font-size: 16px;
​ font-family: Monospace;
​ }
​ 
​ .thick-green-border {
​ border-color: green;
​ border-width: 10px;
​ border-style: solid;
​ border-radius: 50%;
​ }
​ 
​ .smaller-image {
​ width: 100px;
​ }
​ </style>
​ 
​ <h2 class="red-text">CatPhotoApp</h2>
​ 
​ <p>Click here for <a href="#">cat photos</a>.</p>
​ 
​ <a href="#">![](/images/relaxing-cat.jpg)</a>
​ 
​ <p>Things cats love:</p>
​ <ul>
​ <li>cat nip</li>
​ <li>laser pointers</li>
​ <li>lasagna</li>
​ </ul>
​ <p>Top 3 things cats hate:</p>
​ <ol>
​ <li>flea treatment</li>
​ <li>thunder</li>
​ <li>other cats</li>
​ </ol>
​ <form action="/submit-cat-photo">
​ <input type="text" placeholder="cat photo URL">
​ <button type="submit">Submit</button>
​ </form>
​ 
​ Use HTML5 to Require a Field
​ 当你设计表单时，你可以指定某些选项为必填项(required)，只有当用户填写了该选项后，用户才能够提交表单。
​ 
​ 例如，如果你想把一个文本输入字段设置为必填项，在你的input元素中加上required属性就可以了，你可以使用：
​ <input type="text" required>
​ 
​ 任务：给你的输入框添加required属性，这样用户不填写输入框就无法提交表单。
​ 
​ 试试输入框不填写任何文本，然后点击Submit提交表单，看看浏览器如何提示你该字段为必填项。
​ 
​ 注意：required属性在Safari浏览器中不起作用，请用其他浏览器来学习，推荐使用Chrome。
​ 
​ <link href="https://fonts.gdgdocs.org/css?family=Lobster" rel="stylesheet" type="text/css">
​ <style>
​ .red-text {
​ color: red;
​ }
​ 
​ h2 {
​ font-family: Lobster, Monospace;
​ }
​ 
​ p {
​ font-size: 16px;
​ font-family: Monospace;
​ }
​ 
​ .thick-green-border {
​ border-color: green;
​ border-width: 10px;
​ border-style: solid;
​ border-radius: 50%;
​ }
​ 
​ .smaller-image {
​ width: 100px;
​ }
​ </style>
​ 
​ <h2 class="red-text">CatPhotoApp</h2>
​ 
​ <p>Click here for <a href="#">cat photos</a>.</p>
​ 
​ <a href="#">![](/images/relaxing-cat.jpg)</a>
​ 
​ <p>Things cats love:</p>
​ <ul>
​ <li>cat nip</li>
​ <li>laser pointers</li>
​ <li>lasagna</li>
​ </ul>
​ <p>Top 3 things cats hate:</p>
​ <ol>
​ <li>flea treatment</li>
​ <li>thunder</li>
​ <li>other cats</li>
​ </ol>
​ <form action="/submit-cat-photo">
​ <input type="text" placeholder="cat photo URL" required>
​ <button type="submit">Submit</button>
​ </form>
​ 
​ Create a Set of Radio Buttons
​ 类比是最好的学习方式，当你搞不清一个概念时，最好在生活中找到对应的案例。
​ 
​ 单选就是你只能在多个选项中选择一个，就好比你有很多追求者，但却只能选择一个结婚。
​ 
​ 多选一的场景就用radio button(单选按钮)
​ 
​ 单选按钮只是input输入框的一种类型。
​ 
​ 每一个单选按钮都应该嵌套在它自己的label(标签)元素中。
​ 
​ 注意：所有关联的单选按钮应该使用相同的name属性。
​ 
​ 下面是一个单选按钮的例子：
​ 
​ <label><input type="radio" name="indoor-outdoor"> Indoor</label>
​ 
​ 给你的表单添加两个单选按钮，一个叫indoor，另一个叫outdoor。
​ 
​ <link href="https://fonts.gdgdocs.org/css?family=Lobster" rel="stylesheet" type="text/css">
​ <style>
​ .red-text {
​ color: red;
​ }
​ 
​ h2 {
​ font-family: Lobster, Monospace;
​ }
​ 
​ p {
​ font-size: 16px;
​ font-family: Monospace;
​ }
​ 
​ .thick-green-border {
​ border-color: green;
​ border-width: 10px;
​ border-style: solid;
​ border-radius: 50%;
​ }
​ 
​ .smaller-image {
​ width: 100px;
​ }
​ </style>
​ 
​ <h2 class="red-text">CatPhotoApp</h2>
​ 
​ <p>Click here for <a href="#">cat photos</a>.</p>
​ 
​ <a href="#">![](/images/relaxing-cat.jpg)</a>
​ 
​ <p>Things cats love:</p>
​ <ul>
​ <li>cat nip</li>
​ <li>laser pointers</li>
​ <li>lasagna</li>
​ </ul>
​ <p>Top 3 things cats hate:</p>
​ <ol>
​ <li>flea treatment</li>
​ <li>thunder</li>
​ <li>other cats</li>
​ </ol>
​ <form action="/submit-cat-photo">
​ <input type="text" placeholder="cat photo URL" required>
​ <button type="submit">Submit</button>
​ </form>
​ <label>
​ <input type="radio" name="indoor-outdoor">indoor
​ </label>
​ <label>
​ <input type="radio" name="indoor-outdoor">outdoor
​ </label>
​ Create a Set of Checkboxes
​ 当你在大学选课时，面对几百门课程，而因为时间和精力，你只能从中选择十几门。
​ 
​ 这样的场景就用checkboxes（复选按钮）。
​ 
​ 复选按钮是input的输入框的另一种类型。
​ 
​ 每一个复选按钮都应该嵌套进label元素中。
​ 
​ 所有关联的复选按钮应该具有相同的name属性。
​ 
​ 下面是复选按钮的例子：
​ 
​ <label><input type="checkbox" name="personality"> Loving</label>
​ 
​ 任务：为你的表单添加三个复选按钮，每个复选按钮都应该嵌套进它自己的label元素，所有复选按钮的name属性必须为personality。
​ 
​ <link href="https://fonts.gdgdocs.org/css?family=Lobster" rel="stylesheet" type="text/css">
​ <style>
​ .red-text {
​ color: red;
​ }
​ 
​ h2 {
​ font-family: Lobster, Monospace;
​ }
​ 
​ p {
​ font-size: 16px;
​ font-family: Monospace;
​ }
​ 
​ .thick-green-border {
​ border-color: green;
​ border-width: 10px;
​ border-style: solid;
​ border-radius: 50%;
​ }
​ 
​ .smaller-image {
​ width: 100px;
​ }
​ </style>
​ 
​ <h2 class="red-text">CatPhotoApp</h2>
​ 
​ <p>Click here for <a href="#">cat photos</a>.</p>
​ 
​ <a href="#">![](/images/relaxing-cat.jpg)</a>
​ 
​ <p>Things cats love:</p>
​ <ul>
​ <li>cat nip</li>
​ <li>laser pointers</li>
​ <li>lasagna</li>
​ </ul>
​ <p>Top 3 things cats hate:</p>
​ <ol>
​ <li>flea treatment</li>
​ <li>thunder</li>
​ <li>other cats</li>
​ </ol>
​ <form action="/submit-cat-photo">
​ <label><input type="radio" name="indoor-outdoor"> Indoor</label>
​ <label><input type="radio" name="indoor-outdoor"> Outdoor</label>
​ <label><input type="checkbox" name="personality">1</label>
​ <label><input type="checkbox" name="personality">1</label>
​ <label><input type="checkbox" name="personality">1</label>
​ <input type="text" placeholder="cat photo URL" required>
​ <button type="submit">Submit</button>
​ </form>
​ 
​ Check Radio Buttons and Checkboxes by Default
​ 使用checked属性，你可以设置复选按钮和单选按钮默认被选中。
​ 
​ 为此，只需在input元素中添加属性checked
​ 
​ <input type="radio" name="test-name" checked>
​ 
​ 把你的第一个radio button和第一个checkbox都设置为默认选中。
​ 
​ <link href="https://fonts.gdgdocs.org/css?family=Lobster" rel="stylesheet" type="text/css">
​ <style>
​ .red-text {
​ color: red;
​ }
​ 
​ h2 {
​ font-family: Lobster, Monospace;
​ }
​ 
​ p {
​ font-size: 16px;
​ font-family: Monospace;
​ }
​ 
​ .thick-green-border {
​ border-color: green;
​ border-width: 10px;
​ border-style: solid;
​ border-radius: 50%;
​ }
​ 
​ .smaller-image {
​ width: 100px;
​ }
​ </style>
​ 
​ <h2 class="red-text">CatPhotoApp</h2>
​ 
​ <p>Click here for <a href="#">cat photos</a>.</p>
​ 
​ <a href="#">![](/images/relaxing-cat.jpg)</a>
​ 
​ <p>Things cats love:</p>
​ <ul>
​ <li>cat nip</li>
​ <li>laser pointers</li>
​ <li>lasagna</li>
​ </ul>
​ <p>Top 3 things cats hate:</p>
​ <ol>
​ <li>flea treatment</li>
​ <li>thunder</li>
​ <li>other cats</li>
​ </ol>
​ <form action="/submit-cat-photo">
​ <label><input type="radio" name="indoor-outdoor" checked> Indoor</label>
​ <label><input type="radio" name="indoor-outdoor"> Outdoor</label>
​ <label><input type="checkbox" name="personality" checked> Loving</label>
​ <label><input type="checkbox" name="personality"> Lazy</label>
​ <label><input type="checkbox" name="personality"> Energetic</label>
​ <input type="text" placeholder="cat photo URL" required>
​ <button type="submit">Submit</button>
​ </form>
​ 
​ Nest Many Elements within a Single Div Element
​ div元素，也被称作division(层)元素，是一个盛装其他元素的通用容器。
​ 
​ 所以可以利用CSS的继承关系把div上的CSS传递给它所有子元素。
​ 
​ 你可以用<div>来标记一个div元素的开始，然后用</div>来标记一个div元素的结束。
​ 
​ 试着在你的"Things cats love" p元素之前放置div的开始标记，在你的ol结束标记之后放置div的结束标记，这样你的两个列表就都嵌套在div中了。
​ 
​ 把"Things cats love"和"Things cats hate"两个列表都嵌套进同一个div元素中。
​ 
​ <link href="https://fonts.gdgdocs.org/css?family=Lobster" rel="stylesheet" type="text/css">
​ <style>
​ .red-text {
​ color: red;
​ }
​ 
​ h2 {
​ font-family: Lobster, Monospace;
​ }
​ 
​ p {
​ font-size: 16px;
​ font-family: Monospace;
​ }
​ 
​ .thick-green-border {
​ border-color: green;
​ border-width: 10px;
​ border-style: solid;
​ border-radius: 50%;
​ }
​ 
​ .smaller-image {
​ width: 100px;
​ }
​ </style>
​ 
​ <h2 class="red-text">CatPhotoApp</h2>
​ 
​ <p>Click here for <a href="#">cat photos</a>.</p>
​ 
​ <a href="#">![](/images/relaxing-cat.jpg)</a>
​ <div>
​ <p>Things cats love:</p>
​ <ul>
​ <li>cat nip</li>
​ <li>laser pointers</li>
​ <li>lasagna</li>
​ </ul>
​ <p>Top 3 things cats hate:</p>
​ <ol>
​ <li>flea treatment</li>
​ <li>thunder</li>
​ <li>other cats</li>
​ </ol>
​ </div>
​ <form action="/submit-cat-photo">
​ <label><input type="radio" name="indoor-outdoor" checked> Indoor</label>
​ <label><input type="radio" name="indoor-outdoor"> Outdoor</label>
​ <label><input type="checkbox" name="personality" checked> Loving</label>
​ <label><input type="checkbox" name="personality"> Lazy</label>
​ <label><input type="checkbox" name="personality"> Energetic</label>
​ <input type="text" placeholder="cat photo URL" required>
​ <button type="submit">Submit</button>
​ </form>
​ 
​ Give a Background Color to a Div Element
​ 你可以用 background-color 属性来设置一个元素的背景颜色。
​ 
​ 例如，如果你想把一个元素的背景颜色设置为green，你应该把这些加到你的 style 元素中：
​ 
​ .green-background {
​ background-color: green;
​ }
​ 
​ 创建一个叫做 gray-background 的类选择器，设置其 background-color 为 gray，最后应用到 div 元素。
​ 
​ <link href="https://fonts.gdgdocs.org/css?family=Lobster" rel="stylesheet" type="text/css">
​ <style>
​ .red-text {
​ color: red;
​ }
​ 
​ h2 {
​ font-family: Lobster, Monospace;
​ }
​ 
​ p {
​ font-size: 16px;
​ font-family: Monospace;
​ }
​ 
​ .thick-green-border {
​ border-color: green;
​ border-width: 10px;
​ border-style: solid;
​ border-radius: 50%;
​ }
​ 
​ .smaller-image {
​ width: 100px;
​ }
​ 
​ .gray-background {
​ background-color: gray;
​ }
​ </style>
​ 
​ <h2 class="red-text">CatPhotoApp</h2>
​ 
​ <p>Click here for <a href="#">cat photos</a>.</p>
​ 
​ <a href="#">![](/images/relaxing-cat.jpg)</a>
​ 
​ <div class="gray-background">
​ <p>Things cats love:</p>
​ <ul>
​ <li>cat nip</li>
​ <li>laser pointers</li>
​ <li>lasagna</li>
​ </ul>
​ <p>Top 3 things cats hate:</p>
​ <ol>
​ <li>flea treatment</li>
​ <li>thunder</li>
​ <li>other cats</li>
​ </ol>
​ </div>
​ 
​ <form action="/submit-cat-photo">
​ <label><input type="radio" name="indoor-outdoor" checked> Indoor</label>
​ <label><input type="radio" name="indoor-outdoor"> Outdoor</label>
​ <label><input type="checkbox" name="personality" checked> Loving</label>
​ <label><input type="checkbox" name="personality"> Lazy</label>
​ <label><input type="checkbox" name="personality"> Energetic</label>
​ <input type="text" placeholder="cat photo URL" required>
​ <button type="submit">Submit</button>
​ </form>
​ 
​ Set the ID of an Element
​ 除了 class属性之外，每一个 HTML 元素还可以使用 id 属性。
​ 
​ 使用 id 属性有若干好处，一旦当你开始使用 jQuery 的时候你会有更深的体会。
​ 
​ id 属性应该是唯一的，虽然浏览器并不强制唯一，但基于最佳实践，这一点是被广泛认可的，所以请不要给一个以上的元素设置相同的 id 属性。
​ 
​ 下面举例说明了如何设置h2 元素的id属性为cat-photo-app。
​ 
​ <h2 id="cat-photo-app">
​ 
​ 任务：设置 form 元素的id属性为 cat-photo-form。
​ 
​ <link href="https://fonts.gdgdocs.org/css?family=Lobster" rel="stylesheet" type="text/css">
​ <style>
​ .red-text {
​ color: red;
​ }
​ 
​ h2 {
​ font-family: Lobster, Monospace;
​ }
​ 
​ p {
​ font-size: 16px;
​ font-family: Monospace;
​ }
​ 
​ .thick-green-border {
​ border-color: green;
​ border-width: 10px;
​ border-style: solid;
​ border-radius: 50%;
​ }
​ 
​ .smaller-image {
​ width: 100px;
​ }
​ .gray-background {
​ background-color: gray;
​ }
​ </style>
​ 
​ <h2 class="red-text">CatPhotoApp</h2>
​ 
​ <p>Click here for <a href="#">cat photos</a>.</p>
​ 
​ <a href="#">![](/images/relaxing-cat.jpg)</a>
​ 
​ <div class="gray-background">
​ <p>Things cats love:</p>
​ <ul>
​ <li>cat nip</li>
​ <li>laser pointers</li>
​ <li>lasagna</li>
​ </ul>
​ <p>Top 3 things cats hate:</p>
​ <ol>
​ <li>flea treatment</li>
​ <li>thunder</li>
​ <li>other cats</li>
​ </ol>
​ </div>
​ 
​ <form id="cat-photo-form" action="/submit-cat-photo">
​ <label><input type="radio" name="indoor-outdoor" checked> Indoor</label>
​ <label><input type="radio" name="indoor-outdoor"> Outdoor</label>
​ <label><input type="checkbox" name="personality" checked> Loving</label>
​ <label><input type="checkbox" name="personality"> Lazy</label>
​ <label><input type="checkbox" name="personality"> Energetic</label>
​ <input type="text" placeholder="cat photo URL" required>
​ <button type="submit">Submit</button>
​ </form>
​ 
​ Use an ID Attribute to Style an Element
​ 和类选择器一样，你也可以使用ID选择器来声明样式。
​ 
​ 声明一个叫cat-photo-element的ID选择器 ，并设置背景色为绿色。：
​ 
​ #cat-photo-element {
​ background-color: green;
​ }
​ 
​ 注意：在你的 style 元素内部，定义类选择器必须添加 . 为前缀，定义ID选择器必须添加 # 为前缀。
​ 
​ 任务：试着给你的表单，添加一个值为 cat-photo-form的 id 属性，一个绿色的背景。
​ 
​ <link href="https://fonts.gdgdocs.org/css?family=Lobster" rel="stylesheet" type="text/css">
​ <style>
​ .red-text {
​ color: red;
​ }
​ 
​ h2 {
​ font-family: Lobster, Monospace;
​ }
​ 
​ p {
​ font-size: 16px;
​ font-family: Monospace;
​ }
​ 
​ .thick-green-border {
​ border-color: green;
​ border-width: 10px;
​ border-style: solid;
​ border-radius: 50%;
​ }
​ 
​ .smaller-image {
​ width: 100px;
​ }
​ 
​ .gray-background {
​ background-color: gray;
​ }
​ 
​ #cat-photo-form {
​ background-color: green;
​ }
​ </style>
​ 
​ <h2 class="red-text">CatPhotoApp</h2>
​ 
​ <p>Click here for <a href="#">cat photos</a>.</p>
​ 
​ <a href="#">![](/images/relaxing-cat.jpg)</a>
​ 
​ <div class="gray-background">
​ <p>Things cats love:</p>
​ <ul>
​ <li>cat nip</li>
​ <li>laser pointers</li>
​ <li>lasagna</li>
​ </ul>
​ <p>Top 3 things cats hate:</p>
​ <ol>
​ <li>flea treatment</li>
​ <li>thunder</li>
​ <li>other cats</li>
​ </ol>
​ </div>
​ 
​ <form action="/submit-cat-photo" id="cat-photo-form">
​ <label><input type="radio" name="indoor-outdoor" checked> Indoor</label>
​ <label><input type="radio" name="indoor-outdoor"> Outdoor</label>
​ <label><input type="checkbox" name="personality" checked> Loving</label>
​ <label><input type="checkbox" name="personality"> Lazy</label>
​ <label><input type="checkbox" name="personality"> Energetic</label>
​ <input type="text" placeholder="cat photo URL" required>
​ <button type="submit">Submit</button>
​ </form>
​ 
​ Adjusting the Padding of an Element
​ 现在让我们把 Cat Photo App 暂时搁置，以学习更多的 HTML 样式。
​ 
​ 你可能早已经注意到了这点，所有的 HTML 元素本质上是小的矩形块，代表着某一小块区域。
​ 
​ 有三个影响HTML元素布局的重要属性：padding(内边距)、margin(外边距)、border(边框)。
​ 
​ 元素的 padding 控制元素内容 content和元素边框 border之间的距离。
​ 
​ 在这儿，我们可以看到绿方块和红方块都位于黄方块之中，但是红方块比绿方块具有更大的 padding。
​ 
​ 当你加大绿方块的 padding, 它将扩大元素内容和元素边框的距离。
​ 
​ 任务：修改绿方块的 padding 以使它与红方块相匹配。
​ 
​ <style>
​ .injected-text {
​ margin-bottom: -25px;
​ text-align: center;
​ }
​ 
​ .box {
​ border-style: solid;
​ border-color: black;
​ border-width: 5px;
​ text-align: center;
​ }
​ 
​ .yellow-box {
​ background-color: yellow;
​ padding: 10px;
​ }
​ 
​ .red-box {
​ background-color: red;
​ padding: 20px;
​ }
​ 
​ .green-box {
​ background-color: green;
​ padding: 20px;
​ }
​ </style>
​ <h5 class="injected-text">margin</h5>
​ 
​ <div class="box yellow-box">
​ <h5 class="box red-box">padding</h5>
​ <h5 class="box green-box">padding</h5>
​ </div>
​ 
​ Adjust the Margin of an Element
​ 元素的外边距 margin 控制元素边框 border 和元素实际所占空间的距离。
​ 
​ 在这儿，我们可以看到绿方块和红方块都位于黄方块之中，注意红方块比绿方块具有更大的外边距 margin，使得它看起来更小。
​ 
​ 当你增大绿方块的 margin 时，将会增加元素边框和元素实际所占空间之间的距离。
​ 
​ 修改绿方块的 margin 以使它与红方块匹配。
​ 
​ <style>
​ .injected-text {
​ margin-bottom: -25px;
​ text-align: center;
​ }
​ 
​ .box {
​ border-style: solid;
​ border-color: black;
​ border-width: 5px;
​ text-align: center;
​ }
​ 
​ .yellow-box {
​ background-color: yellow;
​ padding: 10px;
​ }
​ 
​ .red-box {
​ background-color: red;
​ padding: 20px;
​ margin: 20px;
​ }
​ 
​ .green-box {
​ background-color: green;
​ padding: 20px;
​ margin: 20px;
​ }
​ </style>
​ <h5 class="injected-text">margin</h5>
​ 
​ <div class="box yellow-box">
​ <h5 class="box red-box">padding</h5>
​ <h5 class="box green-box">padding</h5>
​ </div>
​ 
​ Add a Negative Margin to an Element
​ 元素的 margin 控制元素的 border 和元素实际所占空间的距离。
​ 
​ 如果你将一个元素的 margin 设置为负值，元素将会变大。
​ 
​ 具体可以看看红方块的 margin 值。
​ 
​ 任务：把绿方块的 margin 设置为 -15px，以使它将父容器(黄方块)的横向宽度填满。
​ 
​ <style>
​ .injected-text {
​ margin-bottom: -25px;
​ text-align: center;
​ }
​ 
​ .box {
​ border-style: solid;
​ border-color: black;
​ border-width: 5px;
​ text-align: center;
​ }
​ 
​ .yellow-box {
​ background-color: yellow;
​ padding: 10px;
​ }
​ 
​ .red-box {
​ background-color: red;
​ padding: 20px;
​ margin: -15px;
​ }
​ 
​ .green-box {
​ background-color: green;
​ padding: 20px;
​ margin: -15px;
​ }
​ </style>
​ 
​ <div class="box yellow-box">
​ <h5 class="box red-box">padding</h5>
​ <h5 class="box green-box">padding</h5>
​ </div>
​ 
​ Add Different Padding to Each Side of an Element
​ 有时你想要自定义元素，使它的每一个边具有不同的 padding。
​ 
​ CSS 允许你使用 padding-top、padding-right、padding-bottom 和 padding-left来控制元素上右下左四个方向的 padding。
​ 
​ 使你的绿方块的顶部和左侧具有 40px 的 padding，而底部和右侧则是 20px。
​ 
​ <style>
​ .injected-text {
​ margin-bottom: -25px;
​ text-align: center;
​ }
​ 
​ .box {
​ border-style: solid;
​ border-color: black;
​ border-width: 5px;
​ text-align: center;
​ }
​ 
​ .yellow-box {
​ background-color: yellow;
​ padding: 10px;
​ }
​ 
​ .red-box {
​ background-color: red;
​ padding-top: 40px;
​ padding-right: 20px;
​ padding-bottom: 20px;
​ padding-left: 40px;
​ }
​ 
​ .green-box {
​ background-color: green;
​ padding-top: 40px;
​ padding-right: 20px;
​ padding-left: 40px;
​ padding-bottom:20px;
​ }
​ </style>
​ <h5 class="injected-text">margin</h5>
​ 
​ <div class="box yellow-box">
​ <h5 class="box red-box">padding</h5>
​ <h5 class="box green-box">padding</h5>
​ </div>
​ 
​ Add Different Margins to Each Side of an Element
​ 有时你想要自定义元素，使它的每一个边具有不同的 margin。
​ 
​ CSS 允许你使用 margin-top、margin-right、margin-bottom 和 margin-left 来控制元素上右下左四个方向的 margin。
​ 
​ 使你的绿方块的顶部和左侧具有 40px 的 margin，而底部和右侧则是 20px。
​ 
​ <style>
​ .injected-text {
​ margin-bottom: -25px;
​ text-align: center;
​ }
​ 
​ .box {
​ border-style: solid;
​ border-color: black;
​ border-width: 5px;
​ text-align: center;
​ }
​ 
​ .yellow-box {
​ background-color: yellow;
​ padding: 10px;
​ }
​ 
​ .red-box {
​ background-color: red;
​ margin-top: 40px;
​ margin-right: 20px;
​ margin-bottom: 20px;
​ margin-left: 40px;
​ }
​ 
​ .green-box {
​ background-color: green;
​ margin-top: 40px;
​ margin-right: 20px;
​ margin-bottom: 20px;
​ margin-left: 40px;
​ }
​ </style>
​ <h5 class="injected-text">margin</h5>
​ 
​ <div class="box yellow-box">
​ <h5 class="box red-box">padding</h5>
​ <h5 class="box green-box">padding</h5>
​ </div>
​ 
​ Use Clockwise Notation to Specify the Padding of an Element
​ 除了分别指定元素的 padding-top、padding-right、padding-bottom 和 padding-left 属性外，你还可以集中起来指定它们，举例如下：
​ 
​ padding: 10px 20px 10px 20px;
​ 
​ 这四个值以顺时针方式排列：顶部、右侧、底部、左侧，简称：上右下左。
​ 
​ 使用顺时针方式设置 ".green-box" class，使其顶部和左侧具有 40px 的 padding，而底部和右侧具有 20px 的 padding。
​ 
​ <style>
​ .injected-text {
​ margin-bottom: -25px;
​ text-align: center;
​ }
​ 
​ .box {
​ border-style: solid;
​ border-color: black;
​ border-width: 5px;
​ text-align: center;
​ }
​ 
​ .yellow-box {
​ background-color: yellow;
​ padding: 20px 40px 20px 40px;
​ }
​ 
​ .red-box {
​ background-color: red;
​ padding: 20px 40px 20px 40px;
​ }
​ 
​ .green-box {
​ background-color: green;
​ padding: 40px 20px 20px 40px;
​ }
​ </style>
​ <h5 class="injected-text">margin</h5>
​ 
​ <div class="box yellow-box">
​ <h5 class="box red-box">padding</h5>
​ <h5 class="box green-box">padding</h5>
​ </div>
​ 
​ Use Clockwise Notation to Specify the Margin of an Element
​ 让我们再试一次，但这次是用于 margin。
​ 
​ 除了分别指定元素的 margin-top、margin-right、margin-bottom 和 margin-left 属性外，你还可以集中起来指定它们，举例如下：
​ 
​ margin: 10px 20px 10px 20px;
​ 
​ 这四个值以顺时针方式排列：顶部、右侧、底部、左侧，简称：上右下左。
​ 
​ 使用顺时针表示法设置含有 ".green-box" class 的元素，使其顶部和左侧具有 40px 的 margin，而底部和右侧具有 20px 的 margin。
​ 
​ <style>
​ .injected-text {
​ margin-bottom: -25px;
​ text-align: center;
​ }
​ 
​ .box {
​ border-style: solid;
​ border-color: black;
​ border-width: 5px;
​ text-align: center;
​ }
​ 
​ .yellow-box {
​ background-color: yellow;
​ padding: 20px 40px 20px 40px;
​ }
​ 
​ .red-box {
​ background-color: red;
​ margin: 20px 40px 20px 40px;
​ }
​ 
​ .green-box {
​ background-color: green;
​ margin: 40px 20px 20px 40px;
​ }
​ </style>
​ <h5 class="injected-text">margin</h5>
​ 
​ <div class="box yellow-box">
​ <h5 class="box red-box">padding</h5>
​ <h5 class="box green-box">padding</h5>
​ </div>
​ 
​ Style the HTML Body Element
​ 现在让我们来一个全新的开始，讲一讲 CSS 继承。
​ 
​ 每一个 HTML 页面都有一个 body 元素。
​ 
​ 通过将其 background-color 设置为黑色，我们可以证明 body 元素的存在。
​ 
​ 我们可以通过将下面的代码添加到我们的 style 元素来做到这一点：
​ 
​ body {
​ background-color: black;
​ }
​ 
​ <style>
​ body {
​ background-color: black;
​ }
​ </style>
​ 
​ Inherit Styles from the Body Element
​ 现在我们证明了每一个 HTML 页面都有一个 body 元素，并且其 body 元素同样能够应用样式。
​ 
​ 记住，你可以像对其他 HTML 元素一样对你的 body 元素应用样式，并且所有其他元素将继承你的 body 元素的样式。
​ 
​ 首先，创建一个文字为 Hello World 的 h1 元素。
​ 
​ 然后，让我们通过向 body 元素的样式声明部分添加 color: green; 使页面上的所有元素的颜色为 green。
​ 
​ 最后，通过向 body 元素的样式声明部分添加 font-family: Monospace; 将 body 元素的 font-family（字体）设置为 Monospace。
​ 
​ <style>
​ body {
​ background-color: black;
​ color: green;
​ font-family: Monospace;
​ }
​ 
​ </style>
​ <h1>Hello World</h1>
​ Prioritize One Style Over Another
​ 有时你的 HTML 元素会得到相互冲突的多个样式。
​ 
​ 例如，你的 h1 元素不能同时为绿色和粉色。
​ 
​ 让我们来看看当我们创建一个使其文字为粉色的 class 时会发生什么，然后将其应用到某元素。我们的 class 会 override（覆盖） body 元素的 color: green; CSS 属性吗？
​ 
​ 创建一个使元素颜色成为粉色的名为 pink-text 的 CSS class。
​ 
​ 设置 h1 元素的 class 为 pink-text。
​ 
​ <style>
​ body {
​ background-color: black;
​ font-family: Monospace;
​ color: green;
​ }
​ 
​ .pink-text {
​ color: pink;
​ }
​ </style>
​ <h1 class="pink-text">Hello World!</h1>
​ 
​ Override Styles in Subsequent CSS
​ 我们的 "pink-text" class 覆盖了 body 元素的 CSS 声明！
​ 
​ 我们刚刚证明了我们的 class 会覆盖 body 元素的 CSS，那么下一个合乎情理的问题就是，我们怎样才能覆盖我们的 pink-text class 呢？
​ 
​ 再创建一个把元素设置为蓝色的名为 blue-text 的 CSS class，确保它在你的 pink-text class 声明的下面。
​ 
​ 除了 pink-text class 之外，再把 blue-text class 应用到你的 h1 元素，让我们来看看谁会赢。
​ 
​ 如下例，通过用空格分隔多个 class 属性，可对 HTML 元素应用多个 class 属性：
​ 
​ class="class1 class2"
​ 
​ 注意：在 HTML 中这些 class 如何排序是无所谓的。
​ 
​ 然而，在 <style> 部分中 class 声明的顺序却非常重要，第二个声明总是比第一个具有优先权。因为 .blue-text 是第二个声明，它覆盖了 .pink-text 属性。
​ 
​ <style>
​ body {
​ background-color: black;
​ font-family: Monospace;
​ color: green;
​ }
​ .pink-text {
​ color: pink;
​ }
​ .blue-text {
​ color: blue;
​ }
​ </style>
​ <h1 class="pink-text blue-text">Hello World!</h1>
​ 
​ Override Class Declarations by Styling ID Attributes
​ 我们刚刚证明了浏览器读取 CSS 的顺序是从上到下，这意味着，在发生冲突时，浏览器会使用最后的 CSS 声明。
​ 
​ 但是并非只有这些，还有其他覆盖 CSS 的方法。你还记得 id 属性吗？
​ 
​ 让我们来覆盖你的 pink-text 和 blue-text 两个 class，通过为 h1 元素添加 id 并设置 id 的样式，使你的 h1 元素变成 orange（橙色）。
​ 
​ 给你的 h1 元素添加名为 orange-text 的 id 属性。记住，id 样式看起来是这样的：
​ 
​ <h1 id="orange-text">
​ 
​ 在你的 h1 元素中保留 blue-text 和 pink-text 两个 class。
​ 
​ 在你的 style 元素中为你的 orange-text id 创建一个 CSS 声明，就像下面例子中的样子：
​ 
​ #brown-text {
​ color: brown;
​ }
​ 
​ 注意：你声明的这个 CSS 在 pink-text类选择器的上面还是下面是无所谓的，因为 id 属性总是具有更高的优先级。
​ 
​ <style>
​ body {
​ background-color: black;
​ font-family: Monospace;
​ color: green;
​ }
​ .pink-text {
​ color: pink;
​ }
​ .blue-text {
​ color: blue;
​ }
​ #orange-text {
​ color:orange;
​ }
​ </style>
​ <h1 class="pink-text blue-text" id="orange-text">Hello World!</h1>
​ 
​ Override Class Declarations with Inline Styles
​ 我们证明了无论在 style 元素 CSS 的哪个位置进行声明，id 声明都会覆盖 class 声明。
​ 
​ 还有其他覆盖 CSS 的方法。你还记得行内样式吗？
​ 
​ 试着用 in-line style（行内样式） 使 h1 元素变为白色。记住，行内样式看起来是这样的：
​ 
​ <h1 style="color: green">
​ 
​ 保留 h1 元素中的 blue-text 和 pink-text 两个 class。
​ 
​ <style>
​ body {
​ background-color: black;
​ font-family: Monospace;
​ color: green;
​ }
​ #orange-text {
​ color: orange;
​ }
​ .pink-text {
​ color: pink;
​ }
​ .blue-text {
​ color: blue;
​ }
​ </style>
​ <h1 style="color: white" id="orange-text" class="pink-text blue-text">Hello World!</h1>
​ 
​ Override All Other Styles by using Important
​ 耶！我们刚刚证明了行内样式将覆盖style 中定义的所有 CSS。
​ 
​ 但是等一下，还有最后一种覆盖 CSS 的方法，这是所有方法中最强大的，但是在讲它之前，我们先讲讲为什么你要覆盖 CSS。
​ 
​ 很多情况下，你会使用 CSS 库，这些库可能会意外覆盖掉你自己的 CSS。所以当你需要确保某元素具有指定的 CSS 时，你可以使用 !important。
​ 
​ 让我们再回到我们的 pink-text class 声明。还记得不？我们的 pink-text class 被随后的 class 声明、id 声明和行内样式所覆盖了。
​ 
​ 让我们来给 pink-text 元素的 color 声明加上关键字 !important，以便 100% 确保你的 h1 元素是粉色的。
​ 
​ 举例如下：
​ 
​ color: pink !important;
​ 
​ <style>
​ body {
​ background-color: black;
​ font-family: Monospace;
​ color: green;
​ }
​ #orange-text {
​ color: orange;
​ }
​ .pink-text {
​ color: pink !important;
​ }
​ .blue-text {
​ color: blue;
​ }
​ </style>
​ <h1 id="orange-text" class="pink-text blue-text" style="color: white">Hello World!</h1>
​ 
​ Use Hex Code for Specific Colors
​ 你是否知道在 CSS 中还有其他表示颜色的方法？其中的一种方法称作 hexadecimal code（十六进制编码），简写为 hex code。
​ 
​ 我们通常使用 decimals，也就是十进制数字，它对每一位数字使用符号0到9来表示。Hexadecimals （或 hex）是十六进制数字，这意味着它使用十六个不同的符号。像十进制那样，符号 0-9 代表数值零到九，再使用 A、B、C、D、E、F 代表数值十到十五。合在一起，用 0 到 F 可以代表 hexadecimal 中的每一位数字，共为我们提供 16 个可能的数值。你可以在 这儿 找到更多关于十六进制数字的信息。
​ 
​ 在 CSS 中，我们可以使用 6 位十六进制数字来表示颜色，每 2 位分别表示红色 (R)、绿色 (G) 和蓝色 (B) 成分。例如，#000000 是黑色，同时也是可能的数值中最小的。你可以在 这儿 找到更多关于 RGB 颜色系统的信息。
​ 
​ 把 body 元素的 background-color 由 black 替换成其 hex code 表示，即#000000。
​ 
​ <style>
​ body {
​ background-color: #000000;
​ }
​ </style>
​ 
​ Use Hex Code to Color Elements White
​ 0 是 hex code（十六进制编码）中最小的一个，它代表颜色的完全缺失。
​ 
​ F 是 hex code（十六进制编码）中最大的一个，它代表最大可能的亮度。
​ 
​ 让我们通过把 background-color 的 hex code 修改为 #FFFFFF，以把 body 元素的背景改为白色。
​ 
​ <style>
​ body {
​ background-color: #FFFFFF;
​ }
​ </style>
​ 
​ Use Hex Code to Color Elements Red
​ 你可能会疑惑为什么我们使用6位数来表示一种颜色而不是只用一位或二位，答案是使用6位数可提供给我们巨大数量的颜色变化。
​ 
​ 会有多少种可能的颜色？16 个值和 6 个位置意味着我们有 16 的 6 次方，或者说超过 1600 万种可能的颜色。
​ 
​ Hex code 遵循 red-green-blue（红-绿-蓝），或者叫 rgb 格式。hex code 中的前两位表示颜色中红色的数量，第三四位代表绿色的数量，第五六位代表蓝色的数量。
​ 
​ 所以要得到绝对的纯红色，你只需要在第一和第二位使用 F （最大可能的数值），且在第三、第四、第五和第六位使用 0 （最小可能数值）。
​ 
​ 通过对 background-color 应用 hex code 值 #FF0000以把 body 元素的背景色设置为红色。
​ 
​ <style>
​ body {
​ background-color: #FF0000;
​ }
​ </style>
​ 
​ Use Hex Code to Color Elements Green
​ 记住 hex code 遵循 red-green-blue（红-绿-蓝），或称为 rgb 格式。hex code 中的前两位表示颜色中红色的数量，第三四位代表绿色的数量，第五六位代表蓝色的数量。
​ 
​ 所以要得到绝对的纯绿色，你只需要在第三和第四位使用 F（最大可能的数值），且在其它位使用 0 （最小可能数值）。
​ 
​ 通过对 background-color 应用 hex code 值 #00FF00 以把 body 元素的背景色设置为绿色。
​ 
​ <style>
​ body {
​ background-color: #00FF00;
​ }
​ </style>
​ 
​ Use Hex Code to Color Elements Blue
​ hex code 遵循 red-green-blue（红-绿-蓝），或称为 rgb格式。hex code 中的前两位表示颜色中红色的数量，第三四位代表绿色的数量，第五六位代表蓝色的数量。
​ 
​ 所以要得到绝对的纯蓝色，你只需要在第五和第六位使用 F（最大可能的数值），且在其它位使用 0 （最小可能数值）。
​ 
​ 通过对 background-color 应用 hex code 值 #0000FF 以把 body 元素的背景色设置为蓝色。
​ 
​ <style>
​ body {
​ background-color: #0000FF;
​ }
​ </style>
​ 
​ Use Hex Code to Mix Colors
​ 从这三种纯色（红、绿、蓝），我们能得到 1600 万种其它的颜色。
​ 
​ 例如，橙色是纯红，混合一些绿，没有蓝。
​ 
​ 通过对 background-color 应用 hex code 值 #FFA500 以把 body 元素的背景色设置为橙色
​ 
​ <style>
​ body {
​ background-color: #FFA500;
​ }
​ </style>
​ 
​ Use Hex Code to Color Elements Gray
​ 从这三种纯色（红、绿、蓝），我们能得到 1600 万种其它的颜色。
​ 
​ 我们也可以通过平均混合所有三种颜色得到不同灰度等级的灰色。
​ 
​ 通过对 background-color 应用 hex code 值 #808080 以把 body 元素的背景色设置为灰色。
​ 
​ <style>
​ body {
​ background-color: #808080;
​ }
​ </style>
​ 
​ Use Hex Code for Specific Shades of Gray
​ 通过平均混合所有三种颜色，我们还可以得到其他色度等级的灰色，这样我们可以非常接近纯黑色。
​ 
​ 通过对 background-color 应用 hex code 值 #111111 以把 body 元素的背景色设置为深灰色。
​ 
​ <style>
​ body {
​ background-color: #111111;
​ }
​ </style>
​ 
​ Use Abbreviated Hex Code
​ 许多人对超过 1600 万种颜色感觉十分地抓狂，并且 hex code 非常难以记忆。幸运的是，你可以缩短它。
​ 
​ 例如，红，hex code 是 #FF0000 ，可被缩写成 #F00。也就是说，一位表示红，一位表示绿，一位表示蓝。
​ 
​ 这会把所有可能的颜色数减少至大约 4000 种，但是浏览器会把 #FF0000 和 #F00 解释为完全相同的颜色。
​ 
​ 继续前进，尝试使用 #F00 把 body 元素的背景色改为红色。
​ 
​ <style>
​ body {
​ background-color: #F00;
​ }
​ </style>
​ 
​ Use RGB values to Color Elements
​ 在 CSS 中表示颜色的另一个方法是使用 rgb 值。
​ 
​ 代表黑色的 RGB 值看起来是下面的样子：
​ 
​ rgb(0, 0, 0)
​ 
​ 代表白色的 RGB 值看起来是下面的样子：
​ 
​ rgb(255, 255, 255)
​ 
​ 使用 rgb，你通过 0 至 255 之间的一个数字来指定每种颜色的亮度，而不是像 hex code 那样使用六个十六进制数字。
​ 
​ 如果你做个算术，16 乘以 16 总共有 256 个值，所以从零开始计数的 rgb，和 hex code 一样有完全相同数量的可能数值。
​ 
​ 让我们用黑色的 RGB 值 rgb(0, 0, 0) 替换掉 body 元素背景色的 hex code。
​ 
​ <style>
​ body {
​ background-color: rgb(0,0,0);
​ }
​ </style>
​ 
​ Use RGB to Color Elements White
​ 代表黑色的 RGB 值看起来是下面的样子：
​ 
​ rgb(0, 0, 0)
​ 
​ 代表白色的 RGB 值看起来是下面的样子：
​ 
​ rgb(255, 255, 255)
​ 
​ 使用 rgb，你通过 0 至 255 之间的一个数字来指定每种颜色的亮度，而不是像 hex code 那样使用六个十六进制数字。
​ 
​ 把 body 元素的背景色从黑色的 RGB 值修改为白色的 rgb值 rgb(255, 255, 255)。
​ 
​ <style>
​ body {
​ background-color: rgb(255, 255, 255);
​ }
​ </style>
​ 
​ Use RGB to Color Elements Red
​ 和使用 hex code 一样，你可以通过不同数值的组合来表示 RGB 中不同的颜色。
​ 
​ 这些数值遵循 RGB 顺序模式：第一位表示红色，第二位表示绿色，第三位表示蓝色。
​ 
​ 把 body 元素的背景色修改为红色的 RGB 值：rgb(255, 0, 0)。
​ 
​ <style>
​ body {
​ background-color: rgb(255, 0, 0);
​ }
​ </style>
​ 
​ Use RGB to Color Elements Green
​ 现在将body 元素的背景色修改为绿色的 rgb 值：rgb(0, 255, 0)。
​ 
​ <style>
​ body {
​ background-color: rgb(0, 255, 0);
​ }
​ </style>
​ 
​ Use RGB to Color Elements Blue
​ 将你的 body 元素的背景色修改为蓝色的 RGB 值：rgb(0, 0, 255)。
​ 
​ <style>
​ body {
​ background-color: rgb(0, 0, 255);
​ }
​ </style>
​ 
​ Use RGB to Mix Colors
​ 就像使用 hex code 一样，你可以使用不同数值的组合在 RGB 中混合出各种颜色。
​ 
​ 将 body 元素的背景色修改为橙色的 RGB 值：rgb(255, 165, 0)。
​ 
​ <style>
​ body {
​ background-color: rgb(255, 165, 0);
​ }
​ </style>

