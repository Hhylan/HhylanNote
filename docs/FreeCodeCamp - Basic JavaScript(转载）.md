FreeCodeCamp - Basic JavaScript
（转载）（來源：简书 付林恒 https://www.jianshu.com/p/c9438b1f5ffd）
Comment your JavaScript Code
注释的代码块在JavaScript之中是不会运行的。注释是一个非常好的方式让你自己以及其他人明白这段代码是怎么运行的。

JavaScript中的注释方式有以下两种：

使用 // 来告诉JavaScript来忽略当前行的代码

// This is an in-line comment.

你也可以使用多行注释来注释你的代码，以/*开始，用*/来结束，就像下面这样：

/* This is a
multi-line comment */

最佳实践
你应该给你写的代码添加注释，来让你的代码看起来更加地清晰易懂。良好的注释能够清晰地传达你写的代码的意图—对于那些读你的代码的人来说以及未来你看到它的时候，还能理解这段代码的意图。

任务
尝试创建这两种类型的注释。

// This is an in-line comment.
/* This is an in-line comment */
Declare JavaScript Variables
在计算机科学中, data(数据)就是一切，因为它对于计算机的意义重大。JavaScript提供七种不同的data types(数据类型)，它们是undefined（未定义）, null（空）, boolean（布尔型）, string（字符串）, symbol(符号), number（数字）, and object（对象）。

举个例子, 计算机能够分辨不同的数字, 例如数字 12和 strings，"12"和"dog", 或"123 cats", 都是字母的集合。 计算机能够精确地操作数字， 但是对于字符串却无能为力。

Variables（变量）允许计算机以一种动态的形式来存储和操作数据，通过操作指向数据的指针而不是数据本身来避免了内存泄露，以上的七种数据类型都可以存储到一个变量（variable）中。

Variables 非常类似于你在数学中使用的x,y变量, 这意味着它们都是以一个简单命名的名字来代替我们赋值给它的数据。计算机中的variables（变量）与数学中的变量不同的是，计算机可以在不同的时间存储不同类型的变量。

通过在变量的前面使用关键字var，我们告诉 JavaScript 来创建或者 declare（声明）一个变量,就像这样：

var ourName;

上面代码的意思是创建一个名为ourName的variable（变量），在JavaScript中我们使用分号来结束一段声明。

Variable （变量）的名字可以由数字、字母、$ 或者 _组成，但是不能包含空格或者以数字为首。

任务
使用var 关键字来创建一个名为myName的变量。

提示
如果遇到困难了，请看下ourName的例子是怎么写的。

// 举例
var ourName;

// 请在这条注释以下定义 myName 变量

var myName;
Storing Values with the Equal Operator
在JavaScript中，你可以通过assignment(分配)操作符把一个值存储到变量中。

myVariable = 5;

把Number数字5赋给变量myVariable。

赋值过程是从右到左进行的。所有 = 操作符右边的值都会被赋到左边的变量。

myVar = 5;
myNum = myVar;

数值 5 被赋给变量 myVar 中， 然后变量 myVar又赋给变量 myNum ，这样子 myNum 变量中的值也是 5 了。

任务
把数值 7 赋给变量 a。

把变量 a 中的内容赋给变量 b。

// 初始化变量
var a;
var b = 2;

// 请把你的代码写在这条注释以下
a = 7;
b = a;

Initializing Variables with the Equal Operator
通常地我们会在initialize开始声明变量的时候就会给变量赋一个初始值。

var myVar = 0;

创建一个名为 myVar 的变量并指定一个初始值 0。

任务
通过关键字 var 定义一个变量 a 并且给它一个初始值 9。

// 举例
var ourVar = 19;

// 请把你的代码写在这条注释以下

var a = 9;
Understanding Uninitialized Variables
当 JavaScript 中的变量被声明的时候，程序内部会给它一个初始值 undefined。当你对一个值为 undefined 的变量进行运算操作的时候，算出来的结果将会是 NaN，NaN 的意思是 "Not a Number"。当你用一个没有 定义 的变量来做字符串连接操作的时候，它会如实的输出"undefined"。

任务
定义3个变量 a、b、c ，并且分别给他们赋值：5、10、"I am a" ，这样它们就不会是 undefined（未定义的了）。

// Initialize these three variables
var a = 5;
var b = 10;
var c = "I am a";

// Do not change code below this line

a = a + 1;
b = b + 5;
c = c + " String!";


Understanding Case Sensitivity in Variables
在 JavaScript 中所有的变量都是大小写敏感的。这意味着你要区别对待大写字母和小写字母。

MYVAR与MyVar和myvar 是截然不同的变量。这就有可能导致多个截然不同的变量却有着有相似的名字。正是由于以上原因所以强烈地建议你, 不要 使用这一特性。（以免给自己带来麻烦）

最佳实践
使用 驼峰命名法 来书写一个 Javascript 变量，在 驼峰命名法 中，变量名的第一个单词的首写字母小写，后面的单词的第一个字母大写。

// 初始化变量
var studlyCapVar;
var properCamelCase;
var titleCaseOver;

// 给变量赋值
studlyCapVar = 10;
properCamelCase = "A String";
titleCaseOver = 9000;

Add Two Numbers with JavaScript
现在让我们来尝试在JavaScript中做加法运算。

JavaScript 中使用 + 号来让两个数字执行加法运算。

举例

myVar = 5 + 10; // 等于 15

任务
改变数字 0 让变量 sum 的值为 20.

var sum = 10 + 10;

Subtract One Number from Another with JavaScript
我们也可以在 JavaScript 中执行减法运算。

JavaScript 中使用 - 来做减法运算。

举例

myVar = 12 - 6; // 等于 6

任务
改变数字 0 让变量 difference 的值为 12。

var difference = 45 - 33;

Multiply Two Numbers with JavaScript
我们也可在 JavaScript 中使用乘法运算。

JavaScript 使用这个 * 符号来让两个数字相乘。

举例

myVar = 13 * 13; // 把 169 赋值给 myVar

任务
改变数值 0 来让变量 product 的值等于 80。

var product = 8 * 10;

Divide One Number by Another with JavaScript
我们可以在 JavaScript 中做除法运算。

JavaScript 中使用 / 符号做除法运算。

举例

myVar = 16 / 2; // 把 8 赋值给 myVar

任务
改变数值0来让变量 quotient 的值等于2。

var quotient = 66 / 33;

Increment a Number with JavaScript
使用 ++ ，我们可以很容易地对变量进行自增或者+1运算。

i++;

等效于

i = i + 1;

提示
i++;这种写法，省去了书写=符号的必要。

任务
重写代码，使用 ++ 来对变量 myVar 进行自增操作。

var myVar = 87;

// 请只修改这条注释以下的代码
myVar++;

Decrement a Number with JavaScript
使用自减符号 -- ，你可以很方便地对一个变量执行 自减 或者减一操作。

i--;

等效于

i = i - 1;

提示
i--;这种写法，省去了书写等号的必要。

任务
重写代码，使用 -- 符号对 myVar 执行自减操作。

var myVar = 11;

// 请只修改这条注释以下的代码
myVar--;

Create Decimal Numbers with JavaScript
我们也可以把小数存储到变量中。小数也被称作 浮点数 。

提示
不是所有的实数都可以用 浮点数 来表示。因为可能存在四舍五入的错误，详情在这儿。

任务
创建一个变量 myDecimal 并给它复制一个浮点数。 (e.g. 5.7)。

var ourDecimal = 5.7;

// 请把你的代码写在这条注释以下
var myDecimal = 5.7;

Multiply Two Decimals with JavaScript
在 JavaScript 中，你也可以用小数进行计算，就像整数一样。

让我们把两个小数相乘，并得到它们相乘的结果（product）。

任务
改变 0.0 的数值让变量product的值等于 5.0。

var product = 2.0 * 2.5;

Divide one Decimal by Another with JavaScript
现在让我们来用一个小数做除法操作。

任务
改变数值 0.0 的值让变量 quotient 的值等于 2.2.

var quotient = 4.4 / 2.0;

Finding a Remainder in JavaScript
现在我们用%运算符来取余。

举例

5 % 2 = 1

用法
在数学中，看一个数是奇数还是偶数，只需要看这个数除以2得到的余数是0还是1。

17 % 2 = 1 (17 is 奇数)
48 % 2 = 0 (48 is 偶数)

任务
使用 % 操作符，计算11除以3剩下的余数，并把余数赋给变量remainder。

// 请只修改这条注释以下的代码

var remainder = 11%3;

Assignment with Plus Equals
在编程当中，通常通过赋值来修改变量的内容。请记住，先计算=右边，然后把计算出来的结果赋给左边。

myVar = myVar + 5;

以上是最常见的运算赋值语句，先运算、再赋值。

还有一类操作符是一步到位既做运算也赋值的。

这类操作符的其中一种就是 += 运算符。

myVar += 5; 也是把数值 5 加到变量 myVar上。

任务
使用 += 操作符实现同样的效果。

var a = 3;
var b = 17;
var c = 12;

// 请只修改这条注释以下的代码

a += 12;
b += 9;
c += 7;

Assignment with Minus Equals
与 += 操作符类似，-= 操作符用来对一个变量进行减法赋值操作。

myVar = myVar - 5;

将会从变量 myVar 中减去数值 5。也可以写成这种形式：

myVar -= 5;

任务
使用 -= 操作符实现同样的效果。

var a = 11;
var b = 9;
var c = 3;

// 请只修改这条注释以下的代码

a -= 6;
b -= 15;
c -= 1;

Assignment with Times Equals
*= 操作符是让变量与一个数相乘并赋值。

myVar = myVar * 5;

将会把变量 myVar 与数值 5相乘。也可以写作这样的形式:

myVar *= 5;

任务
使用 *=操作符实现同样的效果。

var a = 5;
var b = 12;
var c = 4.6;

// 请只修改这条注释以下的代码

a *= 5;
b *= 3;
c *= 10;

Assignment with Divided by Equals
/= 操作符是让变量与另一个数相除并赋值。

myVar = myVar / 5;

会把变量 myVar 的值除于 5。等价于:

myVar /= 5;

任务
使用 /=操作符实现同样的效果。

var a = 48;
var b = 108;
var c = 33;

// 请只修改这条注释以下的代码

a /= 12;
b /= 4;
c /= 11;

Convert Celsius to Fahrenheit
为了测试你的学习效果，我们来做一个摄氏度转华氏度的小应用。

从Celsius摄氏度转换为Fahrenheit华氏度的算法是：摄氏度的温度乘于9除于5，再加上32。

创建一个变量 fahrenheit，然后计算出摄氏度对应的华氏度。

function convert(celsius) {
// 请把你的代码写在这条注释以下
fahrenheit = celsius*9/5+32;

// 请把你的代码写在这条注释以上
return fahrenheit;
}

convert(30);  // 你可以修改这一行来测试你的代码

Declare String Variables
先前我们使用过的代码：

var myName = "your name";

"your name" 被称作 字符串。 字符串是用单或双引号包裹起来的一连串的零个或多个字符。

任务
创建两个新的 字符串 变量：myFirstName 和 myLastName 分别为它们赋上你的姓和名的值。

// 举例
var firstName = "Alan";
var lastName = "Turing";

// 请把你的代码写在这条注释以下
var myFirstName = "Frankie";
var myLastName = "Tang";

Escaping Literal Quotes in Strings
当你定义一个字符串必须要用单引号或双引号来包裹它。那么当你需要在字符串中使用一个: " 或者 ' 时该怎么办呢?

在 JavaScript 中，你可以通过在引号前面使用 反斜杠 (\) 来转义引号。

var sampleStr = "Alan said, \"Peter is learning JavaScript\".";

这标志着提醒 JavaScript 单引号或双引号并不是字符串的结尾，而是出现在字符串内的字符。所以，如果你要打印字符串到控制台，你将得到：

Alan said, "Peter is learning JavaScript".

任务
使用 反斜杠 将一个字符串赋值给变量 myStr，以便如果你要打印到控制台，你会看到：

I am a "double quoted" string inside "double quotes"

var myStr = "I am a \"double quoted\" string inside \"double quotes\""; // 请修改这一行

Quoting Strings with Single Quotes
在 JavaScript 中的 字符串 要用单引号或双引号来包裹它，只要你在开始和结束都使用相同类型的引号，单引号和双引号的功能在JavaScript中是相同的。

"This string has \"double quotes\" in it"

当我们需要在字符串中使用与开头结尾相同的引号时，我们需要对引号进行 转义 。如果你有很多双引号的字符串，使用转义字符可能导致难以阅读。这时候可以使用单引号。

'This string has "double quotes" in it. And "probably" lots of them.'

任务
更改myStr字符串的双引号为单引号，并移除转义符号。

var myStr = '<a href="http://www.example.com" target="_blank">Link</a>';

Escape Sequences in Strings
字符串中的转义序列

引号不是字符串中唯一的可以被转义字符。下面是常见的转义序列列表:

Code    Output
'    单引号
"    双引号
\    反斜杠符
\n    换行符
\r    回车符
\t    制表符
\b    退格符
\f    换页符
注意，如果你想要显示一个反斜杠就必须要转义它。

任务
按照下面的顺序，并且用空格来分割：
反斜杠 制表符 退格符 回车符 换行符 并把它赋值给变量 myStr

var myStr = "\\ \t \b \r \n"; // 请修改这一行

Concatenating Strings with Plus Operator
在 JavaScript 中，当 + 操作符与 字符串 一起使用的时候，它被称作 连接 操作符。你可以通过和其他字符串连接 来创建一个新的字符串。

举个例子

'My name is Alan,' + ' I concatenate.'

注意
当心空格。连接操作不会添加两个字符串之外的空格，所以想加上空格的话，你需要自己在字符串里面添加。

任务
使用 + 操作，把字符串 "This is the start. " 和 "This is the end." 连接起来并赋值给变量 myStr。

// 举例
var ourStr = "I come first. " + "I come second.";

// 请只修改这条注释以下的代码

var myStr = "This is the start. " + "This is the end.";

Concatenating Strings with the Plus Equals Operator
我们还可以使用 += 运算符来 连接 字符串到现有字符串的结尾。对于那些非常长的字符串来说，这一操作是非常有用的。

注意
当心空格。连接操作不会添加两个字符串外面的空格，所以如果想要加上空格的话，你需要自己在字符串里面添加。

任务
通过使用 += 操作符来连接这两个字符串:
"This is the first sentence. " 和 "This is the second sentence." 并赋给变量 myStr。

// 举例
var ourStr = "I come first. ";
ourStr += "I come second.";

// 请只修改这条注释以下的代码

var myStr = "This is the first sentence. ";
myStr += "This is the second sentence.";

Constructing Strings with Variables
有时候你需要创建一个填字风格的字符串。

通过使用连接运算符+，你可以插入一个或多个变量来组成一个字符串。

任务
把你的名字赋值给变量 myName ，然后把变量 myName 插入到字符串 "My name is " 和 " and I am swell!"之间，并把连接后的结果赋值给变量 myStr。

// 举例
var ourName = "Free Code Camp";
var ourStr = "Hello, our name is " + ourName + ", how are you?";

// 请只修改这条注释以下的代码
var myName = "Tang Kalun";
var myStr = "My name is " + myName +" and I am swell!";

Appending Variables to Strings
我们不仅可以创建出多行的字符串，还可以使用加等号(+=)运算符来追加变量到字符串上。

任务
设置变量 someAdjective 的值，并使用 += 运算符把它追加到变量 myStr 上。

// 举例
var anAdjective = "awesome!";
var ourStr = "Free Code Camp is ";
ourStr += anAdjective;

// 请只修改这条注释以下的代码

var someAdjective = "a happy thing!";
var myStr = "Learning to code is ";
myStr += someAdjective;

Find the Length of a String
你可以通过在字符串变量或字符串后面写上 .length 来获得字符串变量 字符串 值的长度。

"Alan Peter".length; // 10

例如，我们创建了一个变量 var firstName = "Charles"，我们就可以通过使用 firstName.length 来获得 "Charles" 字符串的长度。

任务
使用 .length 属性来获得变量 lastName 的长度，并把它赋值给变量 lastNameLength。

// 举例
var firstNameLength = 0;
var firstName = "Ada";

firstNameLength = firstName.length;

// 初始化变量
var lastNameLength = 0;
var lastName = "Lovelace";

// 请只修改这条注释以下的代码

lastNameLength = lastName.length;

Use Bracket Notation to Find the First Character in a String
[]叫中括号，{}叫大括号，()叫小括号。

JavaScript中只有字符串类型，没有字符类型。那么如何获取到字符串中的某个字符呢？

我们通过[索引] 来获得对应的字符。

大多数现代编程语言，如JavaScript，不同于人类从1开始计数。它们是从0开始计数，这被称为 基于零 的索引。

例如, 在单词 "Charles" 中索引0上的字符为 "C"，所以在 var firstName = "Charles" 中，你可以使用 firstName[0] 来获得第一个位置上的字符。

任务
使用[索引]来得到变量 lastName 中的第一个字符，并赋给变量 firstLetterOfLastName 。

提示
如果你遇到困难了，不妨看看变量 firstLetterOfFirstName 是如何赋值的。

// 举例
var firstLetterOfFirstName = "";
var firstName = "Ada";

firstLetterOfFirstName = firstName[0];

// 初始化变量
var firstLetterOfLastName = "";
var lastName = "Lovelace";

// 请只修改这条注释以下的代码
firstLetterOfLastName = lastName[0];

Understand String Immutability
理解字符串的不可变性！当你搞懂不可变性后immutable.js对于你就是小菜一碟了。

在 JavaScript 中，字符串 的值是 不可变的，这意味着一旦字符串被创建就不能被改变。

例如，下面的代码：

var myStr = "Bob";
myStr[0] = "J";

是不会把变量 myStr 的值改变成 "Job" 的，因为变量 myStr 是不可变的。注意，这 并不 意味着 myStr 永远不能被改变，只是字符串字面量 string literal 的各个字符不能被改变。改变 myStr 中的唯一方法是重新给它赋一个值，就像这样：

var myStr = "Bob";
myStr = "Job";

任务
把myStr 的值改为Hello World。

// 初始化变量
var myStr = "Jello World";

// 请只修改这条注释以下的代码 原来是myStr[0] = "H" console.log(myStr);/ Jello world

myStr = "Hello World"; // 请修改这一行

Use Bracket Notation to Find the Nth Character in a String
你也可以使用 [索引]来获得一个字符串中的其他位置的字符。

请记住，程序是从 0 开始计数，所以获取第一个字符实际上是[0]。

任务
让我们使用[索引]，把 lastName 变量的第三个字符赋值给 thirdLetterOfLastName。

提示
如果你遇到困难了，看看 secondLetterOfFirstName 变量是如何做的。

// 举例
var firstName = "Ada";
var secondLetterOfFirstName = firstName[1];

// 初始化变量
var lastName = "Lovelace";

// 请只修改这条注释以下的代码
var thirdLetterOfLastName = lastName[2];

Use Bracket Notation to Find the Last Character in a String
为了得到一个字符串的最后一个字符，你可以用[字符串的长度减去一]。

例如，在 var firstName = "Charles" 中，你可以这样操作 firstName[firstName.length - 1] 来得到字符串的最后的一个字符。

任务
使用 [索引] 来取得 lastName 变量中的最后一个字符。

提示
如果你遇到困难了，不妨看看在 lastLetterOfFirstName 变量上是怎么做的。

// 举例
var firstName = "Ada";
var lastLetterOfFirstName = firstName[firstName.length - 1];

// 初始化变量
var lastName = "Lovelace";

// 请只修改这条注释以下的代码
var lastLetterOfLastName = lastName[lastName.length - 1];

Use Bracket Notation to Find the NthtoLast Character in a String
我们既可以获取字符串的最后一个字符，也可以用获取字符串的倒数第N个字符。

例如，你可以这样 firstName[firstName.length - 3] 操作来获得 var firstName = "Charles" 字符串中的倒数第三个字符。

任务
使用 [索引] 来获得 lastName 字符串中的倒数第二个字符。

提示
如果你遇到困难了，不妨看看 thirdToLastLetterOfFirstName 变量是如何做到的。

// 举例
var firstName = "Ada";
var thirdToLastLetterOfFirstName = firstName[firstName.length - 3];

// 初始化变量
var lastName = "Lovelace";

// 请只修改这条注释以下的代码
var secondToLastLetterOfLastName = lastName[lastName.length - 2];

Word Blanks
填词造句

现在，我们来用字符串的相关知识实现一个造句函数。

通过使用提供的变量参数：名词myNoun、形容词myAdjective、动词myVerb、副词myAdverb，来创建一个新的句子 result。

请注意，在英文中，句中的单词是必须用空格来分隔的

举个例子，如果名词为 "dog"，形容词为 "big"，动词为 "run"，副词为"quickly"，那么函数返回值为 "dog big run quickly" 就是没问题的

此外，为了句子通顺，你可以在包含所有传入单词的前提下自己添加一些其他单词。对于上面的例子，函数返回值为 "That big brown dog just run quickly" 也是没问题的

function wordBlanks(myNoun, myAdjective, myVerb, myAdverb) {
var result = "";
// 请把你的代码写在这条注释以下
result = myNoun + " " + myAdjective + " " + myVerb + " " + myAdverb; 

// 请把你的代码写在这条注释以上
return result;
}

wordBlanks("dog", "big", "ran", "quickly");  // 你可以修改这一行来测试你的代码

Store Multiple Values in one Variable using JavaScript Arrays
使用 数组，我们可以在一个地方存储多个数据。

你以左方括号[开始定义一个数组，以右方括号]结束定义，并把每个条目之间用逗号隔开，就像这样：
var sandwich = ["peanut butter", "jelly", "bread"]。

任务
创建一个包含 字符串 和 数字 的数组 myArray。

提示
如果你遇到困难，请参考文本编辑器中的示例代码。

// 举例
var array = ["John", 23];

// 请只修改这条注释以下的代码
var myArray = ["Frankie",21];

Nest one Array within Another Array
你也可以在数组中包含其他数组，就像这样: [["Bulls", 23], ["White Sox", 45]]。这被称为一个 多维数组。

任务
创建一个名为 myArray的多维数组。

// 举例
var ourArray = [["the universe", 42], ["everything", 101010]];

// 请只修改这条注释以下的代码
var myArray = [["dog",20],["cat",21]];

Access Array Data with Indexes
我们可以像操作字符串一样通过数组索引[index]来访问数组中的数据。

数组索引的使用与字符串索引一样，不同的是，通过字符串的索引得到的是一个字符，通过数组索引得到的是一个条目。与字符串类似，数组也是 基于零 的索引，因此数组的第一个元素的索引是 0。

例如

var array = [1,2,3];
array[0]; // 等于 1
var data = array[1]; // 等于 2

任务
创建一个名为 myData 的变量，并把 myArray的第一个索引上的值赋给它。

// 举例
var ourArray = [1,2,3];
var ourData = ourArray[0]; // ourData 的值为 1

// 初始化变量
var myArray = [1,2,3];

// 请把你的代码写在这条注释以下
var myData = myArray[0];

Modify Array Data With Indexes
与字符串的数据不可变不同，数组的数据是可变的，并且可以自由地改变。

例如

var ourArray = [3,2,1];
ourArray[0] = 1; // ourArray等于 [1,2,1]

任务
修改数组 myArray 中索引0上的值为 3。

// 举例
var ourArray = [1,2,3];
ourArray[1] = 3; // ourArray 的值为 [1,3,3].

// 初始化变量
var myArray = [1,2,3];

// 请把你的代码写在这条注释以下
myArray[0] = 3;

Access MultiDimensional Arrays With Indexes
可以把 多维 数组看作成是一个 数组中的数组。当使用[]去访问数组的时候，第一个[index]访问的是第N个子数组，第二个[index]访问的是第N个子数组的第N个元素。

例如

var arr = [
[1,2,3],
[4,5,6],
[7,8,9],
[[10,11,12], 13, 14]
];
arr[0]; // 等于 [1,2,3]
arr[1][2]; // 等于 6
arr[3][0][1]; // 等于 11
任务
使用恰当的 [index] 访问 myArray，使得 myData 的值为 8

// 初始化变量
var myArray = [[1,2,3], [4,5,6], [7,8,9], [[10,11,12], 13, 14]];

// 请只修改这条注释以下的代码
var myData = myArray[2][1];

Manipulate Arrays With push
一个简单的方法将数据追加到一个数组的末尾是通过 push() 函数。

.push() 接受把一个或多个参数，并把它“推”入到数组的末尾。

var arr = [1,2,3];
arr.push(4);
// 现在arr的值为 [1,2,3,4]

任务
把 ["dog", 3] “推”入到 myArray 变量的末尾。

// 举例
var ourArray = ["Stimpson", "J", "cat"];
ourArray.push(["happy", "joy"]); 
// 经过 push 操作后，ourArray 的值为 ["Stimpson", "J", "cat", ["happy", "joy"]]

// 初始化变量
var myArray = [["John", 23], ["cat", 2]];

// 请把你的代码写在这条注释以下
myArray.push(["dog",3]);

Manipulate Arrays With pop
改变数组中数据的另一种方法是用 .pop() 函数。

.pop() 函数用来“抛出”一个数组末尾的值。我们可以把这个“抛出”的值赋给一个变量存储起来。

数组中任何类型的条目（数值，字符串，甚至是数组）可以被“抛出来” 。

举个例子, 对于这段代码
var oneDown = [1, 4, 6].pop();
现在 oneDown 的值为 6 ，数组变成了 [1, 4]。

任务
使用 .pop() 函数移除 myArray 中的最后一条，并且把“抛出”的值赋给 removedFromMyArray。

// 举例
var ourArray = [1,2,3];
var removedFromOurArray = ourArray.pop(); 
// 经过 pop 操作之后，removedFromOurArray 的值为 3, ourArray 的值为 [1,2]

// 初始化变量
var myArray = [["John", 23], ["cat", 2]];

// 请只修改这条注释以下的代码
var removedFromMyArray = myArray.pop();

Manipulate Arrays With shift
pop() 函数用来移出数组中最后一个元素。如果想要移出第一个元素要怎么办呢？

这就是 .shift() 的用武之地。它的工作原理就像 .pop()，但它移除的是第一个元素，而不是最后一个。

任务
使用 .shift() 函数移出 myArray 中的第一项，并把“移出”的值赋给 removedFromMyArray。

// 举例
var ourArray = ["Stimpson", "J", ["cat"]];
removedFromOurArray = ourArray.shift();
// 经过 shift 操作后，removedFromOurArray 的值为 "Stimpson"，ourArray 的值为 ["J", ["cat"]].

// 初始化变量
var myArray = [["John", 23], ["dog", 3]];

// 请只修改这条注释以下的代码
var removedFromMyArray = myArray.shift();

Manipulate Arrays With unshift
你不仅可以 shift（移出）数组中的第一个元素，你也可以 unshift（移入）一个元素到数组的头部。

.unshift() 函数用起来就像 .push() 函数一样, 但不是在数组的末尾添加元素，而是在数组的头部添加元素。

任务
使用 unshift() 函数把["Paul",35] 加入到 myArray 的头部。

// 举例
var ourArray = ["Stimpson", "J", "cat"];
ourArray.shift(); // 经过 shift 操作后，ourArray 的值为 ["J", "cat"]
ourArray.unshift("Happy"); 
// 经过 unshift 操作后，ourArray 的值为 ["Happy", "J", "cat"]

// 初始化变量
var myArray = [["John", 23], ["dog", 3]];
myArray.shift();

// 请把你的代码写在这条注释以下
myArray.unshift(["paul",35]);

Shopping List
购物清单

创建一个名叫 myList的购物清单，清单的数据格式就是多维数组。

每个子数组中的第一个元素应该是购买的物品名称，第二个元素应该是物品的数量，类似于：

["Chocolate Bar", 15]

任务：你的购物清单至少应该有5个子数组。

var myList = [["a",1],["b",1],["c",1],["d",1],["e",1]];

Write Reusable JavaScript with Functions
在 JavaScript 中，我们可以把代码的重复部分抽取出来，放到一个函数（functions）中。

这是一个函数（function）的例子：

function functionName() {
console.log("Hello World");
}

你可以通过函数名称functionName加上后面的小括号来调用这个函数（function），就像这样：

functionName();

每次调用函数时它会打印出消息的“Hello World”到开发的控制台上。所有的大括号之间的代码将在每次函数调用时执行。

任务
创建一个名为 myFunction 的函数，这个函数可以打印“Hi World”到开发控制台上。
调用这个函数。
// 举例
function ourFunction() {
console.log("Heyya, World");
}

ourFunction();

// 请把你的代码写在这条注释以下
function myFunction() {
console.log("Hi World");
}

myFunction();
Passing Values to Functions with Arguments
函数的参数parameters在函数中充当占位符(也叫形参)的作用，参数可以为一个或多个。调用一个函数时所传入的参数为实参，实参决定着形参真正的值。简单理解：形参即形式、实参即内容。

这是带有两个参数的函数， param1 和 param2：

function testFun(param1, param2) {
console.log(param1, param2);
}

接着我们调用 testFun：

testFun("Hello", "World");

我们传递了两个参数， "Hello" 和 "World"。在函数内部，param1 等于“Hello”，param2等于“World”。请注意，testFun 函数可以多次调用，每次调用时传递的参数会决定形参的实际值。

任务
创建一个名为 myFunction 的函数，它可以接收两个参数，计算参数的和，将结果输出到控制台。
调用这个函数。
// 举例
function ourFunction(a, b) {
console.log(a - b);
}
ourFunction(10, 5); // 输出 5

// 请把你的代码写在这条注释以下
function myFunction(a,b) {
console.log(a + b);
}
myFunction(1,2);
Global Scope and Functions
在 JavaScript 中， 作用域 涉及到变量的作用范围。在函数外定义的变量具有 全局 作用域。这意味着，具有全局作用域的变量可以在代码的任何地方被调用。

这些没有使用var关键字定义的变量，会被自动创建在全局作用域中，形成全局变量。当在代码其他地方无意间定义了一个变量，刚好变量名与全局变量相同，这时会产生意想不到的后果。因此你应该总是使用var关键字来声明你的变量。

任务
在函数外声明一个 全局 变量 myGlobal，并给它一个初始值 10

在函数 fun1 的内部，不使用 var 关键字来声明 oopsGlobal，并赋值为 5。

// 请在这里定义变量
var myGlobal = 10;

function fun1() {
// 请在这里把 5 赋值给 oopsGlobal
oopsGlobal = 5;
}

// 请只修改这条注释以上的代码
function fun2() {
var output = "";
if (typeof myGlobal != "undefined") {
output += "myGlobal: " + myGlobal;
}
if (typeof oopsGlobal != "undefined") {
output += " oopsGlobal: " + oopsGlobal;
}
console.log(output);
}

Local Scope and Functions
在一个函数内声明的变量，以及该函数的参数都是局部变量，意味着它们只在该函数内可见。

这是在函数 myTest内声明局部变量loc 的最佳例子：

function myTest() {
var loc = "foo";
console.log(loc);
}
myTest(); // "foo"
console.log(loc); // "undefined"

在函数外，loc 是未定义的。

任务
在函数 myFunction 内部声明一个局部变量 myVar，并删除外部console.log。

function myFunction() {
'use strict';
var myVar = 'use strict';

console.log(myVar);
}
myFunction();

// 请先运行这段代码，并在左边的输出区域或浏览器的控制台中查看输出
// 由于 myVar 在 myFunction 内外均没有定义，因此才会有报错
//console.log(myVar);

// 现在，在 myFunction 中定义 myVar，并删掉 myFunction 外面的 console.log 那一行

Global vs Local Scope in Functions
一个程序中有可能具有相同名称的 局部 变量 和 全局 变量。在这种情况下，局部 变量将会优先于 全局 变量。

下面为例：

var someVar = "Hat";
function myFun() {
var someVar = "Head";
return someVar;
}

函数 myFun 将会返回 "Head"，因为 局部变量 优先级更高。

任务
给 myFunction 添加一个局部变量来覆盖 outerWear 的值为 "sweater"。

// Setup
var outerWear = "T-Shirt";

function myFunction() {
// Only change code below this line

var outerWear = "sweater";

// Only change code above this line
return outerWear;
}

myFunction();

Return a Value from a Function with Return
我们可以把数据通过函数的 参数 来传入函数，也可以使用 return 语句把数据从一个函数中传出来。

例如

function plusThree(num) {
return num + 3;
}
var answer = plusThree(5); // 8

plusThree 带有一个为 num 的 参数 并且返回（returns）一个等于 num + 3 的值。

任务
创建一个函数 timesFive 接受一个参数, 把它乘于 5 之后并返回（returns）。

// 举例
function minusSeven(num) {
return num - 7;
}

// Only change code below this line
function timesFive(num) {
return num * 5;
}

var answer = timesFive(5);
var answer = timesFive(2);
var answer = timesFive(0);
Assignment with a Returned Value
如果你还记得我们在这一节 Storing Values with the Equal Operator 的讨论，赋值之前，先完成等号右边的操作。这意味着我们可把一个函数的返回值，赋值给一个变量。

假设我们预先定义的函数 sum 其功能就是将两个数字相加，那么：

ourSum = sum(5, 12);

将调用 sum 函数，返回return了一个数值 17，然后把它赋值给了 ourSum 变量。

任务
调用 process 函数并给参数一个值 7，然后把返回的值赋值给变量 processed。

// 举例
var changed = 0;

function change(num) {
return (num + 5) / 3;
}

changed = change(10);

// Setup
var processed = 0;

function process(num) {
return (num + 3) / 5;
}

// Only change code below this line
processed = process(7);

Stand in Line
在计算机科学中 队列（queue）是一个抽象的数据结构，队列中的条目都是有秩序的。新的条目会被加到 队列 的末尾，旧的条目会从 队列的头部被移出。

写一个函数 queue ，用一个数组arr和一个数字item作为参数。数字item添加到数组的结尾，然后移出数组的第一个元素，最后队列函数应该返回被删除的元素。

function queue(arr, item) {
// 请把你的代码写在这里
arr.push(item);
item = arr.shift();
return item;  // 请修改这一行
}

// 初始化测试数据
var testArr = [1,2,3,4,5];

// 控制台输出
console.log("Before: " + JSON.stringify(testArr));
console.log(queue(testArr, 6)); // 你可以修改这一行来测试你的代码
console.log("After: " + JSON.stringify(testArr));

JSON.stringify()

Understanding Boolean Values
另一种数据类型是布尔（Boolean）。布尔 值要么是true 要么是false。它非常像电路开关， true 是“开”，false 是“关”。这两种状态是互斥的。

注意
Boolean 值绝不会写作被引号包裹起来的形式。字符串 的 "true" 和 "false" 不是 布尔值，在 JavaScript 中也没有特殊含义。

任务
修改 welcomeToBooleans 函数，让它返回 true而不是 false。

function welcomeToBooleans() {

// Only change code below this line.

return true; // Change this line

// Only change code above this line.
}

Use Conditional Logic with If Statements
If 语句用于在代码中做条件判断。关键字 if告诉 JavaScript 在小括号中的条件为真的情况下去执行定义在大括号里面的代码。这种条件被称为 Boolean 条件，因为他们只可能是 true（真）或 false（假）。

当条件的计算结果为 true，程序执行大括号内的语句。当布尔条件的计算结果为 false，大括号内的代码将不会执行。

伪代码

if(条件为真){
语句被执行
}

示例

function test (myCondition) {
if (myCondition) {
​ return "It was true";
​ }
​ return "It was false";
​ }
​ test(true); // 返回 "It was true"
​ test(false); // 返回 "It was false"
​ 
​ 当 test 被调用，并且传递进来的参数值为 true，if 语句会计算 myCondition 的结果，看它是真还是假。如果条件为 true，函数会返回 "It was true"。当 test 被调用，并且传递进来的参数值为 false，myCondition 不 为 true，并且不执行大括号后面的语句，函数返回 "It was false"。
​ 
​ 任务
​ 在函数内部创建一个 if 语句，如果该参数 wasThatTrue 值为 true，返回 "That was true"，否则，并返回 "That was false"。
​ 
​ // 举例
​ function ourFunction(isItTrue) {
​ if (isItTrue) { 
​ return "Yes, it's true";
​ }
​ return "No, it's false";
​ }
​ 
​ // Setup
​ function myFunction(wasThatTrue) {
​ if (wasThatTrue) {
​ return "That was true";
​ }
​ // Only change code below this line.
​ 
​ return "That was false";
​ 
​ // Only change code above this line.
​ 
​ }
​ 
​ // Change this value to test
​ myFunction(true);
​ 
​ Comparison with the Equality Operator
​ 在 JavaScript 中，有很多 相互比较的操作。所有这些操作符都返回一个 true 或 false值。
​ 
​ 最基本的运算符是相等运算符：==。相等运算符比较两个值，如果它们是同等，返回 true，如果它们不等，返回 false。值得注意的是相等运算符不同于赋值运算符（=），赋值运算符是把等号右边的值赋给左边的变量。
​ 
​ function equalityTest(myVal) {
​ if (myVal == 10) {
​ return "Equal";
​ }
​ return "Not Equal";
​ }
​ 
​ 如果 myVal 等于 10，相等运算符会返回 true，因此大括号里面的代码会被执行，函数将返回 "Equal"。否则，函数返回 "Not Equal"。
​ 
​ 在 JavaScript 中，为了让两个不同的 数据类型（例如 数字 和 字符串）的值可以作比较，它必须把一种类型转换为另一种类型。然而一旦这样做，它可以像下面这样来比较：
​ 
​ 1 == 1 // true
​ 1 == 2 // false
​ 1 == '1' // true
​ "3" == 3 // true
​ 
​ 任务
​ 把 相等运算符 添加到指定的行，这样当 val 的值为12的时候，函数会返回"Equal"。
​ 
​ // Setup
​ function myTest(val) {
​ if (val == 12) { // Change this line
​ return "Equal";
​ }
​ return "Not Equal";
​ }
​ 
​ // Change this value to test
​ myTest(10);
​ 
​ Comparison with the Strict Equality Operator
​ 严格相等运算符（===）是相对于相等操作符（==）的一种操作符。与相等操作符不同的是，它会同时比较元素的值和 数据类型。
​ 
​ 举个例子
​ 
​ 3 === 3 // true
​ 3 === '3' // false
​ 
​ 3 是一个 数字 类型的，而'3' 是一个 字符 类型的，所以3不全等于'3'。
​ 
​ 任务
​ 在 if 语句值使用严格相等运算符，这样当 val严格等于7的时候，函数会返回"Equal"。
​ 
​ // Setup
​ function myTest(val) {
​ if (val === 7) { // Change this line
​ return "Equal";
​ }
​ return "Not Equal";
​ }
​ 
​ // Change this value to test
​ myTest(10);
​ 
​ Comparison with the Inequality Operator
​ 不相等运算符（!=）与相等运算符是相反的。这意味着不相等运算符中，如果“不为真”并且返回 false 的地方，在相等运算符中会返回true，反之亦然。与相等运算符类似，不相等运算符在比较的时候也会转换值的数据类型。
​ 
​ 例如
​ 
​ 1 != 2 // true
​ 1 != "1" // false
​ 1 != '1' // false
​ 1 != true // false
​ 0 != false // false
​ 
​ 任务
​ 在 if 语句中，添加不相等运算符 !=，这样函数在当 val 不等于 99 的时候，会返回 "Not Equal"。
​ 
​ // Setup
​ function myTest(val) {
​ if (val != 99) { // Change this line
​ return "Not Equal";
​ }
​ return "Equal";
​ }
​ 
​ // Change this value to test
​ myTest(10);
​ 
​ Comparison with the Strict Inequality Operator
​ 严格不相等运算符（!==）与全等运算符是相反的。这意味着严格不相等并返回 false 的地方，用严格相等运算符会返回 true，反之亦然。严格相等运算符不会转换值的数据类型。
​ 
​ 例如
​ 
​ 3 !== 3 // false
​ 3 !== '3' // true
​ 4 !== 3 // true
​ 
​ 任务
​ 在 if 语句中，添加严格不相等运算符 !==，这样如果 val 与 17 严格不相等的时候，函数会返回 "Not Equal"。
​ 
​ // Setup
​ function myTest(val) {
​ // Only Change Code Below this Line
​ 
​ if (val !== 17) {
​ 
​ // Only Change Code Above this Line
​ 
​ return "Not Equal";
​ }
​ return "Equal";
​ }
​ 
​ // Change this value to test
​ myTest(10);
​ 
​ Comparison with the Greater Than Operator
​ 使用大于运算符（>）来比较两个数字。如果大于运算符左边的数字大于右边的数字，将会返回 true。否则，它返回 false。
​ 
​ 与相等运算符一样，大于运算符在比较的时候，会转换值的数据类型。
​ 
​ 例如
​ 
​ 5 > 3 // true
​ 7 > '3' // true
​ 2 > 3 // false
​ '1' > 9 // false
​ 
​ 任务
​ 添加 大于 运算符到指定的行，使得返回的语句是有意义的。
​ 
​ function myTest(val) {
​ if (val > 100) {  // Change this line
​ return "Over 100";
​ }
​ 
​ if (val > 10) {  // Change this line
​ return "Over 10";
​ }
​ 
​ return "10 or Under";
​ }
​ 
​ // Change this value to test
​ myTest(10);
​ 
​ Comparison with the Greater Than Or Equal To Operator
​ 使用 大于等于 运算符（>=）来比较两个数字的大小。如果大于等于运算符左边的数字比右边的数字大或者相等，它会返回 true。否则，它会返回 false。
​ 
​ 与相等运算符相似，大于等于 运算符在比较的时候会转换值的数据类型。
​ 
​ 例如
​ 
​ 6 >= 6 // true
​ 7 >= '3' // true
​ 2 >= 3 // false
​ '7' >= 9 // false
​ 
​ 任务
​ 添加 大于等于 运算符到指定行，使得函数的返回语句有意义。
​ 
​ function myTest(val) {
​ if (val >= 20) {  // Change this line
​ return "20 or Over";
​ }
​ 
​ if (val >= 10) {  // Change this line
​ return "10 or Over";
​ }
​ 
​ return "9 or Under";
​ }
​ 
​ // Change this value to test
​ myTest(10);
​ 
​ Comparison with the Less Than Operator
​ 使用 小于 运算符（<）比较两个数字的大小。如果小于运算符左边的数字比右边的数字小，它会返回 true。否则，他会返回 false。与相等运算符类似，小于 运算符在做比较的时候会转换值的数据类型。
​ 
​ 例如
​ 
​ 2 < 5 // true
​ '3' < 7 // true
​ 5 < 5 // false
​ 3 < 2 // false
​ '8' < 4 // false
​ 
​ 任务
​ 添加 小于 运算符到指定行，使得函数的返回语句有意义。
​ 
​ function myTest(val) {
​ if (val < 25) {  // Change this line
​ return "Under 25";
​ }
​ 
​ if (val < 55) {  // Change this line
​ return "Under 55";
​ }
​ 
​ return "55 or Over";
​ }
​ 
​ // Change this value to test
​ myTest(10);
​ 
​ Comparison with the Less Than Or Equal To Operator
​ 使用 小于等于 运算符（<=）比较两个数字的大小。如果在小于等于运算符，左边的数字小于或者等于右边的数字，它会返回 true。如果在小于等于运算符，左边的数字大于或者等于右边的数字，它会返回 false。与相等运算符类型，小于等于 运算符会转换数据类型。
​ 
​ 例如
​ 
​ 4 <= 5 // true
​ '7' <= 7 // true
​ 5 <= 5 // true
​ 3 <= 2 // false
​ '8' <= 4 // false
​ 
​ 任务
​ 添加 小于等于 运算符到指定行，使得函数的返回语句有意义。
​ 
​ function myTest(val) {
​ if (val <= 12) {  // Change this line
​ return "Smaller Than or Equal to 12";
​ }
​ 
​ if (val <= 24) {  // Change this line
​ return "Smaller Than or Equal to 24";
​ }
​ 
​ return "25 or More";
​ }
​ 
​ // Change this value to test
​ myTest(10);
​ 
​ 
​ Comparisons with the Logical And Operator
​ 有时你需要在一次判断中做多个操作。当且仅当运算符的左边和右边都是 true，逻辑与 运算符（&&）才会返回 true。
​ 
​ 同样的效果可以通过if语句的嵌套来实现：
​ 
​ if (num > 5) {
​ if (num < 10) {
​ return "Yes";
​ }
​ }
​ return "No";
​ 
​ 只有当 num 的值在6和9之间（包括6和9）才会返回 "Yes"。相同的逻辑可被写为：
​ 
​ if (num > 5 && num < 10) {
​ return "Yes";
​ }
​ return "No";
​ 
​ 任务
​ 结合两个if语句为一个语句，如果 val 小于或等于 50 并且大于或等于 25，返回 "Yes"。否则，将返回 "No"。
​ 
​ function myTest(val) {
​ // Only change code below this line
​ 
​ if (val <=50 && val >= 25) {
​ return "Yes";
​ }
​ 
​ // Only change code above this line
​ return "No";
​ }
​ 
​ // Change this value to test
​ myTest(10);
​ 
​ Comparisons with the Logical Or Operator
​ 如果任何一个操作数是true，逻辑或 运算符 (||) 返回 true。反之，返回 false。
​ 
​ 举个例子：
​ 
​ if (num > 10) {
​ return "No";
​ }
​ if (num < 5) {
​ return "No";
​ }
​ return "Yes";
​ 
​ 只有当num大于等于5或小于等于10时，函数返回"Yes"。相同的逻辑可以简写成：
​ 
​ if (num > 10 || num < 5) {
​ return "No";
​ }
​ return "Yes";
​ 
​ 任务
​ 结合两个if语句为一个语句，如果val不在10和20之间(包括10和20)，返回 "Outside"。反之，返回 "Inside"。
​ 
​ function myTest(val) {
​ // Only change code below this line
​ 
​ if (val < 10 || val > 20) {
​ return "Outside";
​ }
​ 
​ // Only change code above this line
​ return "Inside";
​ }
​ 
​ // Change this value to test
​ myTest(15);
​ 
​ Introducing Else Statements
​ 当if语句的条件为真，大括号里的代码执行，那如果条件为假呢？
​ 
​ 正常情况下什么也不会发生。
​ 
​ 写一个else语句，当条件为假时执行相应的代码。
​ 
​ if (num > 10) {
​ return "Bigger than 10";
​ } else {
​ return "10 or Less";
​ }
​ 
​ 任务
​ 结合多个if语句为一个if/else语句。
​ 
​ function myTest(val) {
​ var result = "";
​ // Only change code below this line
​ 
​ if (val > 5) {
​ result = "Bigger than 5";
​ } else {
​ result = "5 or Smaller";
​ }
​ 
​ // Only change code above this line
​ return result;
​ }
​ 
​ // Change this value to test
​ myTest(4);
​ 
​ Introducing Else If Statements
​ 如果你有多个条件语句，你可以通过else if语句把 if语句链起来。
​ 
​ if (num > 15) {
​ return "Bigger than 15";
​ } else if (num < 5) {
​ return "Smaller than 5";
​ } else {
​ return "Between 5 and 15";
​ }
​ 
​ 任务
​ 使用else if实现同样的效果。
​ 
​ function myTest(val) {
​ if (val > 10) {
​ return "Greater than 10";
​ } else if (val < 5) {
​ return "Smaller than 5";
​ } else {
​ return "Between 5 and 10";
​ }
​ }
​ // Change this value to test
​ myTest(7);
​ 
​ Logical Order in If Else Statements
​ if、else if语句中代码的执行顺序是很重要的。
​ 
​ 在条件判断语句中，代码的执行顺序是从上到下，所以你需要考虑清楚先执行哪一句，后执行哪一句。
​ 
​ 这有两个例子。
​ 
​ 第一个例子：
​ 
​ function foo(x) {
​ if (x < 1) {
​ return "Less than one";
​ } else if (x < 2) {
​ return "Less than two";
​ } else {
​ return "Greater than or equal to two";
​ }
​ }
​ 
​ 第二个例子更改了代码的执行顺序：
​ 
​ function bar(x) {
​ if (x < 2) {
​ return "Less than two";
​ } else if (x < 1) {
​ return "Less than one";
​ } else {
​ return "Greater than or equal to two";
​ }
​ }
​ 
​ 这两个函数看起来几乎一模一样，我们传一个值进去看看它们有什么区别。
​ 
​ foo(0) // "Less than one"
​ bar(0) // "Less than two"
​ 
​ 任务
​ 更改函数的逻辑顺序以便通过所有的测试用例。
​ 
​ function myTest(val) {
​ if (val < 5) {
​ return "Less than 5";
​ } else if (val < 10) {
​ return "Less than 10";
​ } else {
​ return "Greater than or equal to 10";
​ }
​ }
​ 
​ // Change this value to test
​ myTest(4);
​ 
​ Chaining If Else Statements
​ if/else 语句串联在一起可以实现复杂的逻辑，这是多个if/else if 语句串联在一起的伪代码：
​ 
​ if (condition1) {
​ statement1
​ } else if (condition2) {
​ statement2
​ } else if (condition3) {
​ statement3
​ . . .
​ } else {
​ statementN
​ }
​ 
​ 任务
​ 把if/else if语句串联起来实现下面的逻辑：
​ 
​ num < 5 - return "Tiny"
​ num < 10 - return "Small"
​ num < 15 - return "Medium"
​ num < 20 - return "Large"
​ num >= 20 - return "Huge"
​ 
​ function myTest(num) {
​ // Only change code below this line
​ if (num < 5) {
​ return "Tiny";
​ } else if (num < 10) {
​ return "Small";
​ } else if (num < 15) {
​ return "Medium";
​ } else if (num < 20) {
​ return "Large";
​ } else if (num >= 20) {
​ return "Huge";
​ }
​ 
​ return "Change Me";
​ // Only change code above this line
​ }
​ 
​ // Change this value to test
​ myTest(7);
​ 
​ Golf Code
​ 在高尔夫golf游戏中，每个洞都有自己的标准杆数par，代表着距离。根据你把球打进洞所挥杆的次数strokes，可以计算出你的高尔夫水平。
​ 
​ 函数将会传送2个参数，分别是标准杆数par 和 挥杆次数strokes ，根据下面的表格返回正确的水平段位。
​ 
​ Strokes    Return
​ 1    "Hole-in-one!"
​ <= par - 2    "Eagle"
​ par - 1    "Birdie"
​ par    "Par"
​ par + 1    "Bogey"
​ par + 2    "Double Bogey"
​ >= par + 3    "Go Home!"
​ par 和 strokes 必须是数字而且是正数。
​ 
​ function golfScore(par, strokes) {
​ // Only change code below this line
​ if (strokes == 1) {
​ return "Hole-in-one!";
​ } else if (strokes <= par-2) {
​ return "Eagle";
​ } else if (strokes == par-1) {
​ return "Birdie";
​ } else if (strokes == par) {
​ return "Par";
​ } else if (strokes == par+1) {
​ return "Bogey";
​ } else if (strokes == par+2) {
​ return "Double Bogey";
​ } else if (strokes >= par+3) {
​ return "Go Home!";
​ }
​ 
​ return "Change Me";
​ // Only change code above this line
​ }
​ 
​ // Change these values to test
​ golfScore(5, 4);
​ 
​ Selecting from many options with Switch Statements
​ 如果你有非常多的选项需要选择，可以使用switch语句。根据不同的参数值会匹配上不同的case分支，语句会从第一个匹配的case分支开始执行，直到碰到break就结束。
​ 
​ 这是一个伪代码案例：
​ 
​ switch (num) {
​ case value1:
​ statement1;
​ break;
​ case value2:
​ statement2;
​ break;
​ ...
​ case valueN:
​ statementN;
​ break;
​ }
​ 
​ 测试case 值使用严格相等运算符进行比较，break关键字告诉javascript停止执行语句。如果没有break关键字，下一个语句会继续执行。
​ 
​ 任务
​ 写一个测试 val的switch语句，并且根据下面的条件来设置不同的answer：
​ 1 - "alpha"
​ 2 - "beta"
​ 3 - "gamma"
​ 4 - "delta"
​ 
​ function myTest(val) {
​ var answer = "";
​ // Only change code below this line
​ switch (val) {
​ case 1:
​ answer = "alpha";
​ break;
​ case 2:
​ answer = "beta";
​ break;
​ case 3:
​ answer = "gamma";
​ break;
​ case 4:
​ answer = "delta";
​ break;
​ }
​ // Only change code above this line  
​ return answer;  
​ }
​ 
​ // Change this value to test
​ myTest(1);
​ 
​ Adding a default option in Switch statements
​ 在switch 语句中你可能无法用case来指定所有情况，这时你可以添加default语句。当再也找不到case匹配的时候default语句会执行，非常类似于if/else组合中的else语句。
​ 
​ default语句应该是最后一个case。
​ 
​ switch (num) {
​ case value1:
​ statement1;
​ break;
​ case value2:
​ statement2;
​ break;
​ ...
​ default:
​ defaultStatement;
​ }
​ 
​ 任务
​ 写一个根据下面的条件来设置answer的switch语句：
​ "a" - "apple"
​ "b" - "bird"
​ "c" - "cat"
​ default - "stuff"
​ 
​ function myTest(val) {
​ var answer = "";
​ // Only change code below this line
​ switch (val) {
​ case "a":
​ answer = "apple";
​ break;
​ case "b":
​ answer = "bird";
​ break;
​ case "c":
​ answer = "cat";
​ break;
​ default:
​ answer = "stuff";
​ break;
​ }
​ 
​ // Only change code above this line  
​ return answer;  
​ }
​ 
​ // Change this value to test
​ myTest(1);
​ 
​ Multiple Identical Options in Switch Statements
​ 如果switch语句中的case分支的break 语句漏掉了，后面的 case语句会一直执行直到遇到break。如果你有多个输入值和输出值一样，可以试试下面的switch语句：
​ 
​ switch(val) {
​ case 1:
​ case 2:
​ case 3:
​ result = "1, 2, or 3";
​ break;
​ case 4:
​ result = "4 alone";
​ }
​ 
​ 分支1、2、3将会产生相同的输出结果。
​ 
​ 任务
​ 写一个根据下面的范围来设置answer 的switch语句：
​ 1-3 - "Low"
​ 4-6 - "Mid"
​ 7-9 - "High"
​ 
​ 提示
​ 你需要为每一个包含数字的范围准备一个answer语句。
​ 
​ function myTest(val) {
​ var answer = "";
​ // Only change code below this line
​ switch(val) {
​ case 1:
​ case 2:
​ case 3:
​ answer = "Low";
​ break;
​ case 4:
​ case 5:
​ case 6:
​ answer = "Mid";
​ break;
​ case 7:
​ case 8:
​ case 9: 
​ answer = "High";
​ break;
​ }
​ 
​ // Only change code above this line  
​ return answer;  
​ }
​ 
​ // Change this value to test
​ myTest(1);
​ 
​ Replacing If Else Chains with Switch
​ 如果你有多个选项需要选择，switch 语句写起来会比多个串联的if/if else语句容易些，譬如:
​ 
​ if (val === 1) {
​ answer = "a";
​ } else if (val === 2) {
​ answer = "b";
​ } else {
​ answer = "c";
​ }
​ 
​ 可以被下面替代：
​ 
​ switch (val) {
​ case 1:
​ answer = "a";
​ break;
​ case 2:
​ answer = "b";
​ break;
​ default:
​ answer = "c";
​ }
​ 
​ 任务
​ 把串联的 if/if else 语句改成 switch 语句。
​ 
​ function myTest(val) {
​ var answer = "";
​ // Only change code below this line
​ 
​ switch (val) {
​ case "bob":
​ answer = "Marley";
​ break;
​ case 42:
​ answer = "The Answer";
​ break;
​ case 1:
​ answer = "There is no #1";
​ break;
​ case 99:
​ answer = "Missed me by this much!";
​ break;
​ case 7:
​ answer = "Ate Nine";
​ break;  
​ }
​ // Only change code above this line  
​ return answer;  
​ }
​ 
​ // Change this value to test
​ myTest(7);
​ 
​ Returning Boolean Values from Functions
​ 你可能会回想起Comparison with the Equality Operator ，所有的比较操作符返回的都是一个boolean值，要么是 true 要么是false 。
​ 
​ 使用 if/else语句来做比较然后返回true或false已经成为大家的共识:
​ 
​ function isEqual(a,b) {
​ if (a === b) {
​ return true;
​ } else {
​ return false;
​ }
​ }
​ 
​ 因为=== 总是返回 true 或 false，所以我们可以直接返回比较的结果：
​ 
​ function isEqual(a,b) {
​ return a === b;
​ }
​ 
​ 任务
​ 移除isLess函数的if/else语句但不影响函数的功能。
​ 
​ function isLess(a, b) {
​ // Fix this code
​ return a < b;
​ }
​ 
​ // Change these values to test
​ isLess(10, 15);
​ 
​ Return Early Pattern for Functions
​ 当代码执行到return语句时，函数返回一个结果就结束运行了，return后面的语句根本不会执行。
​ 
​ 举例
​ 
​ function myFun() {
​ console.log("Hello");
​ return "World";
​ console.log("byebye")
​ }
​ myFun();
​ 
​ 上面的代码输出"Hello"到控制台、返回 "World"，但没有输出"byebye"，因为函数遇到return语句就退出了。
​ 
​ 任务
​ 修改函数abTest当a或b小于0时，函数立即返回一个undefined并退出。
​ 
​ 提示
​ 记住undefined，是一个关键字，而不是一个字符串。
​ 
​ // Setup
​ function abTest(a, b) {
​ // Only change code below this line
​ if (a < 0 || b < 0) {
​ return undefined;
​ }
​ 
​ // Only change code above this line
​ 
​ return Math.round(Math.pow(Math.sqrt(a) + Math.sqrt(b), 2));
​ }
​ 
​ // Change values below to test your code
​ abTest(2,2);
​ Math.round()
​ 
​ Math.pow()
​ 
​ Math.sqrt()
​ 
​ Counting Cards
​ 在赌场21点游戏中，玩家可以通过计算牌桌上已经发放的卡牌的高低值来让自己在游戏中保持优势，这就叫21点算法。
​ 
​ 根据下面的表格，每张卡牌都分配了一个值。如果卡牌的值大于0，那么玩家应该追加赌注。反之，追加少许赌注甚至不追加赌注。
​ 
​ Count Change    Cards
​ +1    2, 3, 4, 5, 6
​ 0    7, 8, 9
​ -1    10, 'J', 'Q', 'K','A'
​ 你需要写一个函数，实现21点算法，它根据参数 card的值来递增或递减变量count，函数返回一个由当前count和 "Bet"(count>0)或"Hold"(count<=0) 拼接的字符串。注意count和"Bet"或 "Hold"应该用空格分开。
​ 
​ 例如：
​ "-3 Hold""5 Bet"
​ 
​ 提示
​ 既然card的值为7、8、9时，count值不变，那我们就可以忽略这种情况。
​ 
​ var count = 0;
​ 
​ function cc(card) {
​ // Only change code below this line
​ switch (card) {
​ case 2:
​ case 3:
​ case 4:
​ case 5:
​ case 6:
​ count += 1;
​ break;
​ case 10:
​ case 'J':
​ case 'Q':
​ case 'K':
​ case 'A':
​ count -= 1;
​ break;
​ case 7:
​ case 8:
​ case 9:    
​ count += 0;
​ break;  
​ }
​ if (count > 0) {
​ return count + " Bet";
​ } else {
​ return count + " Hold";
​ }
​ 
​ return "Change Me";
​ // Only change code above this line
​ }
​ 
​ // Add/remove calls to test your function.
​ // 提示: Only the last will display
​ cc(2); cc(3); cc(7); cc('K'); cc('A');
​ 
​ Build JavaScript Objects
​ 你之前可能听说过对象 object 。
​ 
​ 对象和数组很相似，数组是通过索引来访问和修改数据，对象是通过属性来访问和修改数据的。
​ 
​ 这是一个示例对象：
​ 
​ var cat = {
​ "name": "Whiskers",
​ "legs": 4,
​ "tails": 1,
​ "enemies": ["Water", "Dogs"]
​ };
​ 
​ 对象适合用来存储结构化数据，就和真实世界的对象一模一样，比如一只猫。
​ 
​ 任务
​ 创建一个叫做myDog的对象，它里面有这些属性： 名称"name"、 腿"legs", 尾巴"tails"、朋友"friends"。
​ 
​ 你可以设置对象属性为任何你想要的值，只要 "name" 是字符串、 "legs" 和 "tails" 是数字、"friends" 是数组。
​ 
​ // 举例
​ var ourDog = {
​ "name": "Camper",
​ "legs": 4,
​ "tails": 1,
​ "friends": ["everything!"]
​ };
​ 
​ // Only change code below this line.
​ 
​ var myDog = {
​ "name": "wangzhe",
​ "legs": 4,
​ "tails": 0,
​ "friends": ["anything!"]
​ };
​ 
​ Accessing Objects Properties with the Dot Operator
​ 有两种方式访问对象属性，一个是点操作符(.)，一个是中括号操作符([])。
​ 
​ 当你知道属性的名称的时候，使用点操作符。
​ 
​ 这是一个使用点操作符读取对象属性的例子：
​ 
​ var myObj = {
​ prop1: "val1",
​ prop2: "val2"
​ };
​ var prop1val = myObj.prop1; // val1
​ var prop2val = myObj.prop2; // val2
​ 
​ 任务
​ 通过点操作符读取对象testObj，把hat的属性值赋给变量hatValue，把shirt的属性值赋给shirtValue。
​ 
​ // Setup
​ var testObj = {
​ "hat": "ballcap",
​ "shirt": "jersey",
​ "shoes": "cleats"
​ };
​ 
​ // Only change code below this line
​ 
​ var hatValue = testObj.hat;      // Change this line
​ var shirtValue = testObj.shirt;    // Change this line
​ 
​ Accessing Objects Properties with Bracket Notation
​ 第二种访问对象的方式就是中括号操作符([])，如果你想访问的属性的名称有一个空格，这时你只能使用中括号操作符([])。
​ 
​ 这是一个使用中括号操作符([])读取对象属性的例子：
​ 
​ var myObj = {
​ "Space Name": "Kirk",
​ "More Space": "Spock"
​ };
​ myObj["Space Name"]; // Kirk
​ myObj['More Space']; // Spock
​ 
​ 提示：属性名称中如果有空格，必须把属性名称用单引号或双引号包裹起来。
​ 
​ 任务
​ 用中括号操作符读取对象testObj的属性"an entree"值和属性"the drink"值。
​ 
​ // Setup
​ var testObj = {
​ "an entree": "hamburger",
​ "my side": "veggies",
​ "the drink": "water"
​ };
​ 
​ // Only change code below this line
​ 
​ var entreeValue = testObj["an entree"];   // Change this line
​ var drinkValue = testObj["the drink"];    // Change this line
​ Accessing Objects Properties with Variables
​ 中括号操作符的另一个使用方式是用变量来访问一个属性。当你需要遍历对象的属性列表或查表时，这种方式极为有用。
​ 
​ 这有一个使用变量来访问属性的例子：
​ 
​ var someProp = "propName";
​ var myObj = {
​ propName: "Some Value"
​ }
​ myObj[someProp]; // "Some Value"
​ 
​ 还有更多：
​ 
​ var myDog = "Hunter";
​ var dogs = {
​ Fido: "Mutt",
​ Hunter: "Doberman",
​ Snoopie: "Beagle"
​ }
​ var breed = dogs[myDog];
​ console.log(breed)// "Doberman"
​ 
​ 提示：当我们通过变量名访问属性的时候，不需要给变量名包裹引号。因为实际上我们使用的是变量的值，而不是变量的名称。
​ 
​ 任务
​ 使用变量 playerNumber，通过中括号操作符找到 testObj 中 playerNumber 为 16 的值。
​ 
​ // Setup
​ var testObj = {
​ 12: "Namath",
​ 16: "Montana",
​ 19: "Unitas"
​ };
​ 
​ // Only change code below this line;
​ 
​ var playerNumber = 16;       // Change this Line
​ var player = testObj[playerNumber];   // Change this Line
​ 
​ Updating Object Properties
​ 当你创建了一个对象后，你可以用点操作符或中括号操作符来更新对象的属性。
​ 
​ 举个例子，让我们看看 ourDog:
​ 
​ var ourDog = {
​ "name": "Camper",
​ "legs": 4,
​ "tails": 1,
​ "friends": ["everything!"]
​ };
​ 
​ 让我们更改它的名称为 "Happy Camper"，这有两种方式来更新对象的name属性：
​ 
​ ourDog.name = "Happy Camper";
​ 
​ ourDog["name"] = "Happy Camper";
​ 
​ 任务
​ 更新 myDog 对象的name属性，让它的名字从 "Coder" 变成 "Happy Coder"。
​ 
​ // 举例
​ var ourDog = {
​ "name": "Camper",
​ "legs": 4,
​ "tails": 1,
​ "friends": ["everything!"]
​ };
​ 
​ ourDog.name = "Happy Camper";
​ 
​ // Setup
​ var myDog = {
​ "name": "Coder",
​ "legs": 4,
​ "tails": 1,
​ "friends": ["Free Code Camp Campers"]
​ };
​ 
​ // Only change code below this line.
​ myDog.name = "Happy Coder";
​ 
​ Add New Properties to a JavaScript Object
​ 你也可以像更改属性一样给对象添加属性。
​ 
​ 看看我们是如何给ourDog添加 "bark"属性：
​ 
​ ourDog.bark = "bow-wow";
​ 
​ 或者
​ 
​ ourDog["bark"] = "bow-wow";
​ 
​ 任务
​ 给myDog添加一个"bark" 属性，设置它的值为狗的声音，例如："woof"。
​ 
​ // 举例
​ var ourDog = {
​ "name": "Camper",
​ "legs": 4,
​ "tails": 1,
​ "friends": ["everything!"]
​ };
​ 
​ ourDog.bark = "bow-wow";
​ 
​ // Setup
​ var myDog = {
​ "name": "Happy Coder",
​ "legs": 4,
​ "tails": 1,
​ "friends": ["Free Code Camp Campers"]
​ };
​ 
​ // Only change code below this line.
​ myDog.bark = "woof";
​ 
​ Delete Properties from a JavaScript Object
​ 我们同样可以删除对象的属性，例如：
​ 
​ delete ourDog.bark;
​ 
​ 任务
​ 删除myDog对象的"tails"属性。
​ 
​ // 举例
​ var ourDog = {
​ "name": "Camper",
​ "legs": 4,
​ "tails": 1,
​ "friends": ["everything!"],
​ "bark": "bow-wow"
​ };
​ 
​ delete ourDog.bark;
​ 
​ // Setup
​ var myDog = {
​ "name": "Happy Coder",
​ "legs": 4,
​ "tails": 1,
​ "friends": ["Free Code Camp Campers"],
​ "bark": "woof"
​ };
​ 
​ // Only change code below this line.
​ delete myDog.tails;
​ 
​ Using Objects for Lookups
​ 对象和字典一样，可以用来存储键/值对。如果你的数据跟对象一样，你可以用对象来查找你想要的值，而不是使用switch或if/else语句。当你知道你的输入数据在某个范围时，这种查找方式极为有效。
​ 
​ 这是简单的反向字母表：
​ 
​ var alpha = {
​ 1:"Z",
​ 2:"Y",
​ 3:"X",
​ 4:"W",
​ ...
​ 24:"C",
​ 25:"B",
​ 26:"A"
​ };
​ alpha[2]; // "Y"
​ alpha[24]; // "C"
​ var value = 2;
​ alpha[value]; // "Y"
​ 
​ 任务
​ 把switch语句转化为一个叫做lookup的对象。
​ 
​ // Setup
​ function phoneticLookup(val) {
​ var result = "";
​ 
​ // Only change code below this line
​ var lookup = {
​ alpha:"Adams",  
​ bravo:"Boston",
​ charlie:"Chicago",
​ delta:"Denver",
​ echo:"Easy",
​ foxtrot:"Frank",
​ "":undefined  
​ };
​ 
​ // Only change code above this line
​ return lookup[val];
​ }
​ 
​ // Change this value to test
​ phoneticLookup("charlie");
​ 
​ Testing Objects for Properties
​ 有时检查一个对象属性是否存在是非常有用的，我们可以用.hasOwnProperty(propname)方法来检查对象是否有该属性。如果有返回true，反之返回 false。
​ 
​ 举例
​ 
​ var myObj = {
​ top: "hat",
​ bottom: "pants"
​ };
​ myObj.hasOwnProperty("top"); // true
​ myObj.hasOwnProperty("middle"); // false
​ 
​ 任务
​ 修改函数checkObj检查myObj是否有checkProp属性，如果属性存在，返回属性对应的值，如果不存在，返回 "Not Found"。
​ 
​ 注意：如果你需要通过变量来访问对象的属性值，请用中括号操作符，点操作符不支持变量。
​ 
​ // Setup
​ var myObj = {
​ gift: "pony",
​ pet: "kitten",
​ bed: "sleigh"
​ };
​ 
​ function checkObj(checkProp) {
​ // Your Code Here
​ if (myObj.hasOwnProperty(checkProp)) {
​ return myObj[checkProp];
​ } else {
​ return "Not Found";
​ }
​ }
​ 
​ // Test your code by modifying these values
​ checkObj("gift");
​ 
​ Introducing JavaScript Object Notation JSON
​ JavaScript Object Notation 简称 JSON，它使用JavaScript对象的格式来存储数据。JSON是灵活的，因为它允许 数据结构 是 字符串，数字，布尔值，字符串，和 对象 的任意组合。
​ 
​ 这里是一个JSON对象的示例：
​ 
​ var ourMusic = [
​ {
​ "artist": "Daft Punk",
​ "title": "Homework",
​ "release_year": 1997,
​ "formats": [
​ "CD",
​ "Cassette",
​ "LP" ],
​ "gold": true
​ }
​ ];
​ 
​ 这是一个对象数组，并且对象有各种关于专辑的 详细信息。它也有一个嵌套的 formats 的数组。附加专辑记录可以被添加到数组的最上层。
​ 
​ 提示
​ 数组中有多个 JSON 对象的时候，对象与对象之间要用逗号隔开。
​ 
​ 任务
​ 添加一个新专辑到 myMusic 的JSON对象。添加 artist 和 title 字符串，release_year 数字和 formats 字符串数组。
​ 
​ var myMusic = [
​ {
​ "artist": "Billy Joel",
​ "title": "Piano Man",
​ "release_year": 1973,
​ "formats": [ 
​ "CS", 
​ "8T", 
​ "LP" ],
​ "gold": true
​ },//这里很重要，要有逗号隔开。
​ // Add record here
​ {
​ "artist": "Daft Punk",
​ "title": "Homework",
​ "release_year": 1997,
​ "formats": [ 
​ "CD", 
​ "Cassette", 
​ "LP" ],
​ "gold": true
​ }
​ ];
​ Accessing Nested Objects in JSON
​ // Setup
​ var myStorage = {
​ "car": {
​ "inside": {
​ "glove box": "maps",
​ "passenger seat": "crumbs"
​ },
​ "outside": {
​ "trunk": "jack"
​ }
​ }
​ };
​ 
​ // Only change code below this line
​ 
​ var gloveBoxContents = myStorage.car.inside["glove box"]; // Change this line
​ 
​ Accessing Nested Arrays in JSON
​ 正如我们在前面的例子所见，JSON对象可以嵌套对象和数组。与访问嵌套对象一样，用中括号操作符同样可以访问嵌套数组。
​ 
​ 下面是如何访问嵌套数组的例子：
​ 
​ var ourPets = {
​ "cats": [
​ "Meowzer",
​ "Fluffy",
​ "Kit-Cat"
​ ],
​ "dogs": [
​ "Spot",
​ "Bowser",
​ "Frankie"
​ ]
​ };
​ ourPets.cats[1]; // "Fluffy"
​ ourPets.dogs[0]; // "Spot"
​ 
​ 任务
​ 使用点操作符和中括号操作符来检索变量 myPlants 的第二棵树。
​ 
​ // Setup
​ var myPlants = [
​ { 
​ type: "flowers",
​ list: [
​ "rose",
​ "tulip",
​ "dandelion"
​ ]
​ },
​ {
​ type: "trees",
​ list: [
​ "fir",
​ "pine",
​ "birch"
​ ]
​ }  
​ ];
​ 
​ // Only change code below this line
​ 
​ var secondTree = myPlants[1].list[1]; // Change this line
​ 
​ Record Collection
​ 右边有一个JSON对象，代表着你的专辑集。每一张专辑由一个唯一的id标识，并具有多种属性。但并非所有的专辑都有完整的信息。
​ 
​ 写一个函数，它有个三个参数，id、prop、 value。
​ 
​ 如果 value !='' 而且prop != 'tracks' ，collectionCopy[id][prop]=value;。
​ 
​ 如果 value !='' 而且prop == 'tracks' ，collectionCopy[id][prop].push(value);。
​ 
​ 如果 value == '' ，delete collectionCopy[id][prop];。
​ 
​ 记住：函数返回的永远是整个对象。
​ 
​ 提示
​ 使用中括号操作符来 访问对象的变量属性。
​ 
​ // 初始化变量
​ var collection = {
​ 2548: {
​ album: "Slippery When Wet",
​ artist: "Bon Jovi",
​ tracks: [ 
​ "Let It Rock", 
​ "You Give Love a Bad Name" 
​ ]
​ },
​ 2468: {
​ album: "1999",
​ artist: "Prince",
​ tracks: [ 
​ "1999", 
​ "Little Red Corvette" 
​ ]
​ },
​ 1245: {
​ artist: "Robert Palmer",
​ tracks: [ ]
​ },
​ 5439: {
​ album: "ABBA Gold"
​ }
​ };
​ // 深拷贝 collection，用于测试
​ var collectionCopy = JSON.parse(JSON.stringify(collection));
​ 
​ // 请只修改这条注释以下的代码
​ function update(id, prop, value) {
​ if (prop == "tracks" && value) {
​ collection[id][prop].push(value);
​ } else if (value) {
​ collection[id][prop] = value;
​ } else {
​ delete collection[id][prop];
​ }
​ return collection;
​ }
​ 
​ // 你可以修改这一行来测试你的代码
​ update(5439, "artist", "ABBA");
​ 
​ Iterate with JavaScript For Loops
​ 一个条件语句只能执行一次代码，而一个循环语句可以多次执行代码。
​ 
​ JavaScript 中最常见的循环就是“for循环”。
​ 
​ for循环中的三个表达式用分号隔开：
​ 
​ for ([初始化]; [条件判断]; [计数器])
​ 
​ 初始化语句只会在执行循环开始之前执行一次。它通常用于定义和设置你的循环变量。
​ 
​ 条件判断语句会在每一轮循环的开始执行，只要条件判断为 true 就会继续执行循环。当条件为 false的时候，循环将停止执行。这意味着，如果条件在一开始就为 false，这个循环将不会执行。
​ 
​ 计数器是在每一轮循环结束时执行，通常用于递增或递减。
​ 
​ 在下面的例子中，先初始化i = 0，条件 i < 5为真，进入第一次循环，执行大括号里的代码，第一次循环结束。递增i的值，条件判断，就这样依次执行下去，直到条件判断为假，整个循环结束。
​ 
​ var ourArray = [];
​ for (var i = 0; i < 5; i++) {
​ ourArray.push(i);
​ }
​ 
​ 最终 ourArray 的值为 [0,1,2,3,4].
​ 
​ 任务
​ 使用 for 循环把从 1 到 5 添加进 myArray 中。
​ 
​ for循环就是if条件语句的进化版。
​ 
​ // 举例
​ var ourArray = [];
​ 
​ for (var i = 0; i < 5; i++) {
​ ourArray.push(i);
​ }
​ 
​ // Setup
​ var myArray = [];
​ for (var i = 1; i < 6; i++) {
​ myArray.push(i);
​ }
​ // Only change code below this line.
​ 
​ Iterate Odd Numbers With a For Loop
​ for循环可以按照我们指定的顺序来迭代，通过更改我们的 计数器，我们可以按照偶数顺序来迭代。
​ 
​ 初始化 i = 0，当 i < 10 的时候继续循环。
​ 
​ i += 2 让 i 每次循环之后增加2。
​ 
​ var ourArray = [];
​ for (var i = 0; i < 10; i += 2) {
​ ourArray.push(i);
​ }
​ 
​ 循环结束后，ourArray 的值为 [0,2,4,6,8]。
​ 
​ 改变 计数器，这样我们可以用奇数来数。
​ 
​ 任务
​ 写一个 for 循环，把从1到9的奇数添加到 myArray。
​ 
​ // 举例
​ var ourArray = [];
​ 
​ for (var i = 0; i < 10; i += 2) {
​ ourArray.push(i);
​ }
​ 
​ // Setup
​ var myArray = [];
​ 
​ for (var i = 1; i < 10; i += 2) {
​ myArray.push(i);
​ }
​ // Only change code below this line.
​ 
​ Count Backwards With a For Loop
​ for循环也可以逆向迭代，只要我们定义好合适的条件。
​ 
​ 为了能够从后往前两两倒数，我们需要改变我们的 初始化，条件判断 和 计数器。
​ 
​ 我们让 i = 10，并且当 i > 0 的时候才继续循环。我们使用 i-=2 来让 i 每次循环递减 2。
​ 
​ var ourArray = [];
​ for (var i=10; i > 0; i-=2) {
​ ourArray.push(i);
​ }
​ 
​ 循环结束后，ourArray 的值为 [10,8,6,4,2]。
​ 
​ 让我们改变 初始化 和 计数器，这样我们就可以按照奇数从后往前两两倒着数。
​ 
​ 任务
​ 使用一个 for 循环，把9到1的奇数添加进 myArray。
​ 
​ // 举例
​ var ourArray = [];
​ 
​ for (var i = 10; i > 0; i -= 2) {
​ ourArray.push(i);
​ }
​ 
​ // Setup
​ var myArray = [];
​ 
​ for (var i = 9; i > 0; i -= 2) {
​ myArray.push(i);
​ }
​ // Only change code below this line.
​ 
​ Iterate Through an Array with a For Loop
​ 迭代输出一个数组的每个元素是 JavaScript 中的常见需求， for 循环可以做到这一点。
​ 
​ 下面的代码将输出数组 arr 的每个元素到控制台：
​ 
​ var arr = [10,9,8,7,6];
​ for (var i=0; i < arr.length; i++) {
​ console.log(arr[i]);
​ }
​ 
​ 记住数组的索引从零开始的，这意味着数组的最后一个元素的下标是：数组的长度 - 1。我们这个循环的 条件 是 i < arr.length，当 i 的值为 长度-1 的时候循环就停止了。
​ 
​ 任务
​ 声明并初始化一个变量 total 为 0。使用 for循环，使得 total 的值为 myArr 的数组中的每个元素的值的总和。
​ 
​ // 举例
​ var ourArr = [ 9, 10, 11, 12];
​ var ourTotal = 0;
​ 
​ for (var i = 0; i < ourArr.length; i++) {
​ ourTotal += ourArr[i];
​ }
​ 
​ // Setup
​ var myArr = [ 2, 3, 4, 5, 6];
​ var total = 0;
​ 
​ for (var i = 0; i < myArr.length; i++) {
​ total += myArr[i];
​ }
​ // Only change code below this line
​ 
​ Nesting For Loops
​ 如果你有一个二维数组，可以使用相同的逻辑，先遍历外面的数组，再遍历里面的子数组。下面是一个例子：
​ 
​ var arr = [
​ [1,2], [3,4], [5,6]
​ ];
​ for (var i=0; i < arr.length; i++) {
​ for (var j=0; j < arr[i].length; j++) {
​ console.log(arr[i][j]);
​ }
​ }
​ 
​ 一次输出 arr 中的每个子元素。提示，对于内部循环，我们可以通过 arr[i] 的 .length 来获得子数组的长度，因为 arr[i] 的本身就是一个数组。
​ 
​ 任务
​ 修改函数 multiplyAll，获得 arr 内部数组的每个数字相乘的结果 product。
​ 
​ function multiplyAll(arr) {
​ var product = 1;
​ // Only change code below this line
​ for (var i = 0; i < arr.length; i++) {
​ for (var j = 0; j < arr[i].length; j++)
​ product *= arr[i][j];
​ }
​ // Only change code above this line
​ return product;
​ }
​ 
​ // Modify values below to test your code
​ multiplyAll([[1,2],[3,4],[5,6,7]]);
​ 
​ Iterate with JavaScript While Loops
​ 另一种类型的 JavaScript 循环被称为while循环，因为它规定，当（while）条件为真，循环才会执行，反之不执行。
​ 
​ var ourArray = [];
​ var i = 0;
​ while(i < 5) {
​ ourArray.push(i);
​ i++;
​ }
​ 
​ 任务
​ 通过一个 while 循环，把从 0 到 4 的值添加到 myArray 中。
​ 
​ // Setup
​ var myArray = [];
​ var i = 0;
​ while(i < 5) {
​ myArray.push(i);
​ i++;
​ }
​ // Only change code below this line.
​ Profile Lookup
​ 我们有一个对象数组，里面存储着通讯录。
​ 
​ 函数 lookUp 有两个预定义参数：firstName值和prop属性 。
​ 
​ 函数将会检查通讯录中是否存在一个与传入的 firstName 相同的联系人。如果存在，那么还需要检查对应的联系人中是否存在 prop属性。
​ 
​ 如果它们都存在，函数返回prop属性对应的值。
​ 
​ 如果firstName 值不存在，返回 "No such contact"。
​ 
​ 如果prop 属性不存在，返回 "No such property"。
​ 
​ //Setup
​ var contacts = [
​ {
​ "firstName": "Akira",
​ "lastName": "Laine",
​ "number": "0543236543",
​ "likes": ["Pizza", "Coding", "Brownie Points"]
​ },
​ {
​ "firstName": "Harry",
​ "lastName": "Potter",
​ "number": "0994372684",
​ "likes": ["Hogwarts", "Magic", "Hagrid"]
​ },
​ {
​ "firstName": "Sherlock",
​ "lastName": "Holmes",
​ "number": "0487345643",
​ "likes": ["Intriguing Cases", "Violin"]
​ },
​ {
​ "firstName": "Kristian",
​ "lastName": "Vos",
​ "number": "unknown",
​ "likes": ["Javascript", "Gaming", "Foxes"]
​ }
​ ];
​ 
​ function lookUp(firstName, prop){
​ // Only change code below this line
​ for (i = 0; i < contacts.length; i++) {
​ if (contacts[i].firstName == firstName) {
​ if (contacts[i].hasOwnProperty(prop)) {
​ return contacts[i][prop];
​ }
​ return "No such property";
​ }
​ }
​ return "No such contact";
​ // Only change code above this line
​ }
​ 
​ // Change these values to test your function
​ lookUp("Akira", "likes");
​ 
​ Generate Random Fractions with JavaScript
​ 计算机的行为只有两种：确定性和随机性。当你一步步地闯关来到这里就是确定行为，当你随意点了个链接就来到这里就是随机行为。
​ 
​ 而随机数最适合用来创建这种随机行为。
​ 
​ Math.random()用来生成一个在0(包括0)到1(不包括1)之间的随机小数，因此Math.random()可能返回0但绝不会返回1。
​ 
​ 提示
​ 随后的函数都会在return执行前调用，所以我们可以直接返回Math.random()的值。
​ 
​ 任务
​ 更改myFunction 来生成一个随机数取代 0。
​ 
​ function myFunction() {
​ 
​ // Only change code below this line.
​ var myFunction = Math.random();
​ return myFunction;
​ 
​ // Only change code above this line.
​ }
​ 
​ Generate Random Whole Numbers with JavaScript
​ 生成随机小数很棒，但随机数更有用的地方在于生成随机整数。
​ 
​ 用 Math.random() 生成一个随机小数。
​ 把这个随机小数乘以 20。
​ 用 Math.floor() 向下取整 获得它最近的整数。
​ 记住 Math.random() 永远不会返回 1。同时因为我们是在用 Math.floor() 向下取整，所以最终我们获得的结果不可能有 20。这确保了我们获得了一个在0到19之间的整数。
​ 
​ 把操作连缀起来，代码类似于下面：
​ 
​ Math.floor(Math.random() * 20);
​ 
​ 我们先调用 Math.random()，把它的结果乘以20，然后把上一步的结果传给 Math.floor()，最终通过向下取整获得最近的整数。
​ 
​ var randomNumberBetween0and19 = Math.floor(Math.random() * 20);
​ 
​ function myFunction() {
​ 
​ // Only change code below this line.
​ 
​ return Math.floor(Math.random() * 10);
​ 
​ }
​ 
​ Generate Random Whole Numbers within a Range
​ 我们之前生成的随机数是在0到某个数之间，现在我们要生成的随机数是在两个指定的数之间。
​ 
​ 我们需要定义一个最小值和一个最大值。
​ 
​ 下面是我们将要使用的方法，仔细看看并尝试理解这行代码到底在干嘛：
​ 
​ Math.floor(Math.random() * (max - min + 1)) + min
​ 
​ 任务
​ 创建一个叫randomRange的函数，参数为myMin和myMax，返回一个在myMin(包括myMin)和myMax(包括myMax)之间的随机数。
​ 
​ // 举例
​ function ourFunction(ourMin, ourMax) {
​ 
​ return Math.floor(Math.random() * (ourMax - ourMin + 1)) + ourMin;
​ }
​ 
​ ourFunction(1, 9);
​ 
​ // Only change code below this line.
​ 
​ function randomRange(myMin, myMax) {
​ 
​ return Math.floor(Math.random() * (myMax - myMin + 1)) + myMin; // Change this line
​ 
​ }
​ 
​ // Change these values to test your function
​ var myRandom = randomRange(5, 15);
​ 
​ Sift through Text with Regular Expressions
​ Regular expressions 正则表达式被用来根据某种匹配模式来寻找strings中的某些单词。
​ 
​ 举例：如果我们想要找到字符串The dog chased the cat中单词 the，我们可以使用下面的正则表达式: /the/gi
​ 
​ 我们可以把这个正则表达式分成几段：
​ 
​ / 是这个正则表达式的头部
​ 
​ the 是我们想要匹配的模式
​ 
​ / 是这个正则表达式的尾部
​ 
​ g 代表着 global(全局)，意味着返回所有的匹配而不仅仅是第一个。
​ 
​ i 代表着忽略大小写，意思是当我们寻找匹配的字符串的时候忽略掉字母的大小写。
​ 
​ 任务
​ 用全局、忽略大小写的模式选取字符串 testString中所有的单词 and。
​ 
​ 你可以尝试把 . 替换成 and。
​ 
​ // Setup
​ var testString = "Ada Lovelace and Charles Babbage designed the first computer and the software that would have run on it.";
​ 
​ // 举例
​ var expressionToGetSoftware = /software/gi;
​ var softwareCount = testString.match(expressionToGetSoftware).length;
​ 
​ 
​ // Only change code below this line.
​ 
​ var expression = /and/gi;  // Change this Line
​ // Only change code above this line
​ 
​ // This code counts the matches of expression in testString
​ var andCount = testString.match(expression).length;
​ 
​ Find Numbers with Regular Expressions
​ 我们可以在正则表达式中使用特殊选择器来选取特殊类型的值。
​ 
​ 特殊选择器中的一种就是数字选择器\d，意思是被用来获取一个字符串的数字。
​ 
​ 在JavaScript中, 数字选择器类似于: /\d/g。
​ 
​ 在选择器后面添加一个加号标记(+)，例如：/\d+/g，它允许这个正则表达式匹配一个或更多数字。
​ 
​ 尾部的g是'global'的简写，意思是允许这个正则表达式 找到所有的匹配而不是仅仅找到第一个匹配。
​ 
​ 任务
​ 用 \d 选择器来选取字符串中的所有数字。
​ 
​ // Setup
​ var testString = "There are 3 cats but 4 dogs.";
​ 
​ // Only change code below this line.
​ 
​ var expression = /\d+/g;  // Change this line
​ 
​ // Only change code above this line
​ 
​ // This code counts the matches of expression in testString
​ var digitCount = testString.match(expression).length;
​ 
​ Find Whitespace with Regular Expressions
​ 我们也可以使用正则表达式选择器 \s 来选择一个字符串中的空白。
​ 
​ 空白字符有 " " (空格符)、\r (回车符)、\n (换行符)、\t (制表符) 和 \f (换页符)。
​ 
​ 空白正则表达式类似于：
​ 
​ /\s+/g
​ 
​ 任务
​ 用 \s 选取句子中的所有空白字符。
​ 
​ // Setup
​ var testString = "How many spaces are there in this sentence?";
​ 
​ // Only change code below this line.
​ 
​ var expression = /\s+/g;  // Change this line
​ 
​ // Only change code above this line
​ 
​ // This code counts the matches of expression in testString
​ var spaceCount = testString.match(expression).length;
​ 
​ Invert Regular Expression Matches with JavaScript
​ 你可以用正则表达式选择器的大写版本 来转化任何匹配。
​ 
​ 举个例子：\s 匹配任何空白字符，\S 匹配任何非空白字符。
​ 
​ 任务
​ 用 /\S/g 来匹配字符串testString中的所有非空白字符。
​ 
​ // Setup
​ var testString = "How many non-space characters are there in this sentence?";
​ 
​ // Only change code below this line.
​ 
​ var expression = /\S/g;  // Change this line
​ 
​ // Only change code above this line
​ 
​ // This code counts the matches of expression in testString
​ var nonSpaceCount = testString.match(expression).length;
​ 
​ Create a JavaScript Slot Machine
​ 现在把我们之前的所学的知识点结合起来完成一个老虎机游戏。
​ 
​ 这次我们生成3个随机数，范围在1到3之间。
​ 
​ 分别用 slotOne、slotTwo、slotThree来存储着3个随机数。
​ 
​ 用我们之前的所学来生成随机数)：
​ 
​ Math.floor(Math.random() * (3 - 1 + 1)) + 1;
​ 
​ <script>
​ function runSlots() {
​ var slotOne;
​ var slotTwo;
​ var slotThree;
​ 
​ var images = ["//i.imgur.com/9H17QFk.png", "//i.imgur.com/9RmpXTy.png", "//i.imgur.com/VJnmtt5.png"];
​ 
​ // Only change code below this line.
​ 
​ var slotOne = Math.floor(Math.random() * (3 - 1 + 1)) + 1;
​ var slotTwo = Math.floor(Math.random() * (3 - 1 + 1)) + 1;
​ var slotThree = Math.floor(Math.random() * (3 - 1 + 1)) + 1;
​ 
​ // Only change code above this line.
​ 
​ 
​ if (slotOne !== undefined && slotTwo !== undefined && slotThree !== undefined) {
​ $(".logger").html(slotOne + " " + slotTwo + " " + slotThree);
​ }
​ 
​ 
​ $(".logger").append(" Not A Win")
​ return [slotOne, slotTwo, slotThree];
​ }
​ 
​ $(document).ready(function() {
​ $(".go").click(function() {
​ runSlots();
​ });
​ });
​ </script>
​ 
​ <div>
​ <div class = "container inset">
​ <div class = "header inset">
​ ![](/images/freecodecamp_logo.svg)
​ <h2>FCC Slot Machine</h2>
​ </div>
​ <div class = "slots inset">
​ <div class = "slot inset">
​ 
​ </div>
​ <div class = "slot inset">
​ 
​ </div>
​ <div class = "slot inset">
​ 
​ </div>
​ </div>
​ <br/>
​ <div class = "outset">
​ <button class = "go inset">
​ Go
​ </button>
​ </div>
​ <br/>
​ <div class = "foot inset">
​ <span class = "logger"></span>
​ </div>
​ </div>
​ </div>
​ 
​ <style>
​ .container {
​ background-color: #4a2b0f;
​ height: 400px;
​ width: 260px;
​ margin: 50px auto;
​ border-radius: 4px;
​ }
​ .header {
​ border: 2px solid #fff;
​ border-radius: 4px;
​ height: 55px;
​ margin: 14px auto;
​ background-color: #457f86
​ }
​ .header h2 {
​ height: 30px;
​ margin: auto;
​ }
​ .header h2 {
​ font-size: 14px;
​ margin: 0 0;
​ padding: 0;
​ color: #fff;
​ text-align: center;
​ }
​ .slots{
​ display: flex;
​ background-color: #457f86;
​ border-radius: 6px;
​ border: 2px solid #fff;
​ }
​ .slot{
​ flex: 1 0 auto;
​ background: white;
​ height: 75px;
​ margin: 8px;
​ border: 2px solid #215f1e;
​ border-radius: 4px;
​ }
​ .go {
​ width: 100%;
​ color: #fff;
​ background-color: #457f86;
​ border: 2px solid #fff;
​ border-radius: 2px;
​ box-sizing: none;
​ outline: none!important;
​ }
​ .foot {
​ height: 150px;
​ background-color: 457f86;
​ border: 2px solid #fff;
​ }
​ 
​ .logger {
​ color: white;
​ margin: 10px;
​ }
​ 
​ .outset {
​ -webkit-box-shadow: 0px 0px 15px -2px rgba(0,0,0,0.75);
​ -moz-box-shadow: 0px 0px 15px -2px rgba(0,0,0,0.75);
​ box-shadow: 0px 0px 15px -2px rgba(0,0,0,0.75);
​ }
​ 
​ .inset {
​ -webkit-box-shadow: inset 0px 0px 15px -2px rgba(0,0,0,0.75);
​ -moz-box-shadow: inset 0px 0px 15px -2px rgba(0,0,0,0.75);
​ box-shadow: inset 0px 0px 15px -2px rgba(0,0,0,0.75);
​ }
​ </style>
​ 
​ Add your JavaScript Slot Machine Slots
​ 现在我们的老虎机每次生存3个随机数，我们得去检查随机数是否全部相等的情况。
​ 
​ 如果全部相等，我们应该提示用户他们赢了，并返回中奖号码，否则我们应该返回null。
​ 
​ null 是JavaScript中的一种数据类型，意味着空。
​ 
​ 当这3个随机数相等的时候，判定用户赢。让我们创建一个if statement，用多个条件按顺序来检查它们是否相等。类似于：
​ 
​ if (slotOne === slotTwo && slotTwo === slotThree){
​ 
​ return slotOne;
​ 
​ } else {
​ 
​ }
​ 
​ 当3个随机数都一样的时候，我们把 "It's A Win" 追加到class logger的html中。
​ 
​ <script>
​ function runSlots() {
​ var slotOne;
​ var slotTwo;
​ var slotThree;
​ 
​ var images = ["//i.imgur.com/9H17QFk.png", "//i.imgur.com/9RmpXTy.png", "//i.imgur.com/VJnmtt5.png"];
​ 
​ slotOne = Math.floor(Math.random() * (3 - 1 + 1)) + 1;
​ slotTwo = Math.floor(Math.random() * (3 - 1 + 1)) + 1;
​ slotThree = Math.floor(Math.random() * (3 - 1 + 1)) + 1;
​ 
​ 
​ // 请把你的代码写在这条注释以下
​ 
​ if ((slotOne !== slotTwo) || (slotTwo !== slotThree) || (slotThree !== slotOne)) return null;
​ 
​ // 请把你的代码写在这条注释以上
​ 
​ if (slotOne !== undefined && slotTwo !== undefined && slotThree !== undefined){
​ $(".logger").html(slotOne + " " + slotTwo + " " + slotThree);
​ }
​ 
​ $(".logger").append(" It's A Win");
​ 
​ return [slotOne, slotTwo, slotThree];
​ }
​ 
​ $(document).ready(function() {
​ $(".go").click(function() {
​ runSlots();
​ });
​ });
​ </script>
​ 
​ <div>
​ <div class = "container inset">
​ <div class = "header inset">
​ ![](/images/freecodecamp_logo.svg)
​ <h2>FCC Slot Machine</h2>
​ </div>
​ <div class = "slots inset">
​ <div class = "slot inset">
​ 
​ </div>
​ <div class = "slot inset">
​ 
​ </div>
​ <div class = "slot inset">
​ 
​ </div>
​ </div>
​ <br/>
​ <div class = "outset">
​ <button class = "go inset">
​ Go
​ </button>
​ </div>
​ <br/>
​ <div class = "foot inset">
​ <span class = "logger"></span>
​ </div>
​ </div>
​ </div>
​ 
​ <style>
​ .container {
​ background-color: #4a2b0f;
​ height: 400px;
​ width: 260px;
​ margin: 50px auto;
​ border-radius: 4px;
​ }
​ .header {
​ border: 2px solid #fff;
​ border-radius: 4px;
​ height: 55px;
​ margin: 14px auto;
​ background-color: #457f86
​ }
​ .header h2 {
​ height: 30px;
​ margin: auto;
​ }
​ .header h2 {
​ font-size: 14px;
​ margin: 0 0;
​ padding: 0;
​ color: #fff;
​ text-align: center;
​ }
​ .slots{
​ display: flex;
​ background-color: #457f86;
​ border-radius: 6px;
​ border: 2px solid #fff;
​ }
​ .slot{
​ flex: 1 0 auto;
​ background: white;
​ height: 75px;
​ margin: 8px;
​ border: 2px solid #215f1e;
​ border-radius: 4px;
​ }
​ .go {
​ width: 100%;
​ color: #fff;
​ background-color: #457f86;
​ border: 2px solid #fff;
​ border-radius: 2px;
​ box-sizing: none;
​ outline: none!important;
​ }
​ .foot {
​ height: 150px;
​ background-color: 457f86;
​ border: 2px solid #fff;
​ }
​ 
​ .logger {
​ color: white;
​ margin: 10px;
​ }
​ 
​ .outset {
​ -webkit-box-shadow: 0px 0px 15px -2px rgba(0,0,0,0.75);
​ -moz-box-shadow: 0px 0px 15px -2px rgba(0,0,0,0.75);
​ box-shadow: 0px 0px 15px -2px rgba(0,0,0,0.75);
​ }
​ 
​ .inset {
​ -webkit-box-shadow: inset 0px 0px 15px -2px rgba(0,0,0,0.75);
​ -moz-box-shadow: inset 0px 0px 15px -2px rgba(0,0,0,0.75);
​ box-shadow: inset 0px 0px 15px -2px rgba(0,0,0,0.75);
​ }
​ </style>
​ 
​ Bring your JavaScript Slot Machine to Life
​ 让我们用 jQuery 选择器 $(".slot") 获得所有老虎机。
​ 
​ 一旦获取到所有老虎机，我们可以通过中括号操作符获取到每一个老虎机：
​ 
​ $($(".slot")[0]).html(slotOne);
​ 
​ jQuery将会获取到第一个老虎机，并更新它的HTML为正确的数字。
​ 
​ 任务：分别更新每个老虎机上的HTML为对应的数字。
​ 
​ <script>
​ function runSlots() {
​ var slotOne;
​ var slotTwo;
​ var slotThree;
​ 
​ var images = ["//i.imgur.com/9H17QFk.png", "//i.imgur.com/9RmpXTy.png", "//i.imgur.com/VJnmtt5.png"];
​ 
​ slotOne = Math.floor(Math.random() * (3 - 1 + 1)) + 1;
​ slotTwo = Math.floor(Math.random() * (3 - 1 + 1)) + 1;
​ slotThree = Math.floor(Math.random() * (3 - 1 + 1)) + 1;
​ 
​ 
​ // Only change code below this line.
​ 
​ $($(".slot")[0]).html(slotOne);
​ $($(".slot")[1]).html(slotTwo);
​ $($(".slot")[2]).html(slotThree);
​ 
​ // Only change code above this line.
​ 
​ if (slotOne === slotTwo && slotTwo === slotThree) {
​ $(".logger").html(slotOne + " " + slotTwo + " " + slotThree + " It's A Win")
​ return null;
​ }
​ 
​ if (slotOne !== undefined && slotTwo !== undefined && slotThree !== undefined){
​ $(".logger").html(slotOne + " " + slotTwo + " " + slotThree);
​ }
​ 
​ $(".logger").append(" Not A Win");
​ 
​ 
​ return [slotOne, slotTwo, slotThree];
​ }
​ 
​ $(document).ready(function() {
​ $(".go").click(function() {
​ runSlots();
​ });
​ });
​ </script>
​ 
​ <div>
​ <div class = "container inset">
​ <div class = "header inset">
​ ![](/images/freecodecamp_logo.svg)
​ <h2>FCC Slot Machine</h2>
​ </div>
​ <div class = "slots inset">
​ <div class = "slot inset">
​ 
​ </div>
​ <div class = "slot inset">
​ 
​ </div>
​ <div class = "slot inset">
​ 
​ </div>
​ </div>
​ <br/>
​ <div class = "outset">
​ <button class = "go inset">
​ Go
​ </button>
​ </div>
​ <br/>
​ <div class = "foot inset">
​ <span class = "logger"></span>
​ </div>
​ </div>
​ </div>
​ 
​ <style>
​ .container {
​ background-color: #4a2b0f;
​ height: 400px;
​ width: 260px;
​ margin: 50px auto;
​ border-radius: 4px;
​ }
​ .header {
​ border: 2px solid #fff;
​ border-radius: 4px;
​ height: 55px;
​ margin: 14px auto;
​ background-color: #457f86
​ }
​ .header h2 {
​ height: 30px;
​ margin: auto;
​ }
​ .header h2 {
​ font-size: 14px;
​ margin: 0 0;
​ padding: 0;
​ color: #fff;
​ text-align: center;
​ }
​ .slots{
​ display: flex;
​ background-color: #457f86;
​ border-radius: 6px;
​ border: 2px solid #fff;
​ }
​ .slot{
​ flex: 1 0 auto;
​ background: white;
​ height: 75px;
​ margin: 8px;
​ border: 2px solid #215f1e;
​ border-radius: 4px;
​ text-align: center;
​ padding-top: 25px;
​ }
​ .go {
​ width: 100%;
​ color: #fff;
​ background-color: #457f86;
​ border: 2px solid #fff;
​ border-radius: 2px;
​ box-sizing: none;
​ outline: none!important;
​ }
​ .foot {
​ height: 150px;
​ background-color: 457f86;
​ border: 2px solid #fff;
​ }
​ 
​ .logger {
​ color: white;
​ margin: 10px;
​ }
​ 
​ .outset {
​ -webkit-box-shadow: 0px 0px 15px -2px rgba(0,0,0,0.75);
​ -moz-box-shadow: 0px 0px 15px -2px rgba(0,0,0,0.75);
​ box-shadow: 0px 0px 15px -2px rgba(0,0,0,0.75);
​ }
​ 
​ .inset {
​ -webkit-box-shadow: inset 0px 0px 15px -2px rgba(0,0,0,0.75);
​ -moz-box-shadow: inset 0px 0px 15px -2px rgba(0,0,0,0.75);
​ box-shadow: inset 0px 0px 15px -2px rgba(0,0,0,0.75);
​ }
​ </style>
​ 
​ Give your JavaScript Slot Machine some Stylish Images
​ 现在给我们的老虎机加点图片。
​ 
​ 我们已经为你准备好了图片images，我们可以通过不同的索引来获取每个图片。
​ 
​ 现在让我们设置第一个老虎机根据随机数来显示一张图片：
​ 
​ $($('.slot')[0]).html('<img src = "' + images[slotOne-1] + '">');
​ 
​ 任务：设置所有的老虎机根据随机数来显示对应的图片，最后点击RUN。
​ 
​ <script>
​ function runSlots() {
​ var slotOne;
​ var slotTwo;
​ var slotThree;
​ 
​ var images = ["//i.imgur.com/9H17QFk.png", "//i.imgur.com/9RmpXTy.png", "//i.imgur.com/VJnmtt5.png"];
​ 
​ slotOne = Math.floor(Math.random() * (3 - 1 + 1)) + 1;
​ slotTwo = Math.floor(Math.random() * (3 - 1 + 1)) + 1;
​ slotThree = Math.floor(Math.random() * (3 - 1 + 1)) + 1;
​ 
​ 
​ // Only change code below this line.
​ 
​ $($('.slot')[0]).html('<img src = "' + images[slotOne-1] + '">');
​ $($('.slot')[1]).html('<img src = "' + images[slotTwo-1] + '">');
​ $($('.slot')[2]).html('<img src = "' + images[slotThree-1] + '">');
​ 
​ // Only change code above this line.
​ 
​ if (slotOne === slotTwo && slotTwo === slotThree) {
​ $('.logger').html(slotOne + " " + slotTwo + " " + slotThree + "It's A Win");
​ return null;
​ }
​ 
​ if (slotOne !== undefined && slotTwo !== undefined && slotThree !== undefined){
​ $(".logger").html(slotOne + " " + slotTwo + " " + slotThree);
​ }
​ 
​ $('.logger').append(" Not A Win");
​ 
​ return [slotOne, slotTwo, slotThree];
​ }
​ 
​ $(document).ready(function() {
​ $('.go').click(function() {
​ runSlots();
​ });
​ });
​ </script>
​ 
​ <div>
​ <div class = 'container inset'>
​ <div class = 'header inset'>
​ ![](/images/freecodecamp_logo.svg)
​ <h2>FCC Slot Machine</h2>
​ </div>
​ <div class = 'slots inset'>
​ <div class = 'slot inset'>
​ 
​ </div>
​ <div class = 'slot inset'>
​ 
​ </div>
​ <div class = 'slot inset'>
​ 
​ </div>
​ </div>
​ <br/>
​ <div class = 'outset'>
​ <button class = 'go inset'>
​ Go
​ </button>
​ </div>
​ <br/>
​ <div class = 'foot inset'>
​ <span class = 'logger'></span>
​ </div>
​ </div>
​ </div>
​ 
​ <style>
​ .slot > img {
​ margin: 0!important;
​ height: 71px;
​ width: 50px;
​ }
​ .container {
​ background-color: #4a2b0f;
​ height: 400px;
​ width: 260px;
​ margin: 50px auto;
​ border-radius: 4px;
​ }
​ .header {
​ border: 2px solid #fff;
​ border-radius: 4px;
​ height: 55px;
​ margin: 14px auto;
​ background-color: #457f86
​ }
​ .header h2 {
​ height: 30px;
​ margin: auto;
​ }
​ .header h2 {
​ font-size: 14px;
​ margin: 0 0;
​ padding: 0;
​ color: #fff;
​ text-align: center;
​ }
​ .slots{
​ display: flex;
​ background-color: #457f86;
​ border-radius: 6px;
​ border: 2px solid #fff;
​ }
​ .slot{
​ flex: 1 0 auto;
​ background: white;
​ height: 75px;
​ width: 50px;
​ margin: 8px;
​ border: 2px solid #215f1e;
​ border-radius: 4px;
​ text-align: center;
​ }
​ .go {
​ width: 100%;
​ color: #fff;
​ background-color: #457f86;
​ border: 2px solid #fff;
​ border-radius: 2px;
​ box-sizing: none;
​ outline: none!important;
​ }
​ .foot {
​ height: 150px;
​ background-color: 457f86;
​ border: 2px solid #fff;
​ }
​ 
​ .logger {
​ color: white;
​ margin: 10px;
​ }
​ 
​ .outset {
​ -webkit-box-shadow: 0px 0px 15px -2px rgba(0,0,0,0.75);
​ -moz-box-shadow: 0px 0px 15px -2px rgba(0,0,0,0.75);
​ box-shadow: 0px 0px 15px -2px rgba(0,0,0,0.75);
​ }
​ 
​ .inset {
​ -webkit-box-shadow: inset 0px 0px 15px -2px rgba(0,0,0,0.75);
​ -moz-box-shadow: inset 0px 0px 15px -2px rgba(0,0,0,0.75);
​ box-shadow: inset 0px 0px 15px -2px rgba(0,0,0,0.75);
​ }
​ </style>
​ 
​ 很遗憾的是。。
​ 
​ 墙外的 FCC 已经没了老虎机这个项目了。。
​ 
​ 不知道去哪了。。
​ 
