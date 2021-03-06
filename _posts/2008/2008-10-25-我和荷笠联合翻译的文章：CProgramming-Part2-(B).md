---
layout: post
title: 我和荷笠联合翻译的文章：CProgramming-Part2 (B)
categories:
- Diandian
tags:
- Linux

---
<p>Loops and things</p>
<p>The example code has been written so that the most common loop/decisions constructs are used. In this section, 'statements1;' means any sequence of application logic. The first and most common structure can be seen from line 13 to 28 and line 49 to 56, and has the following structure:</p>
<p>循环和事物</p>
<p>示例代码已经写出了，所以最普遍的循环\判断建构被使用。在这个部分中，“语句1”意味着任何应用程序逻辑序列。第一个和最常见的结构能够从13行到28行和49行到56行看出，有一下结构：</p>
<p>if(condition1)<br />{<br />&nbsp;&nbsp;&nbsp; statements1;<br />}<br />else if(condition2)<br />{<br />&nbsp;&nbsp;&nbsp; statements2;<br />}<br />else<br />{<br />&nbsp;&nbsp;&nbsp; statements3;<br />}<br /><br /><br /><br />if（表达式1）<br />{<br />&nbsp;&nbsp;语句1；<br />}<br />else if（表达式2）<br />{<br />&nbsp;&nbsp;语句2；<br />}<br />else<br />{<br />&nbsp;&nbsp;语句3；<br />}<br /></p>
<p>If condition1 is true, statements1 will be executed, otherwise condition2 will be checked; if this is true, statements2 will be executed, and, if all else fails, statements3 will be executed. Both the else if and else' parts are optional, and you can also add more else if'' parts. A condition is considered true when it differs from zero - which explains line 49.</p>
<p>A special form of the if...else structure is on line 27. This form isn't that common, and is typically used for very compact things. Here, it is a compact way of saying that the function should return 0 if count is a divisor or prime, or 1 otherwise.</p>
<p>A first loop is a while loop, for example lines 23 to 26. Here, the body of the loop will be executed provided and as long as the condition is true, which means it is potentially not executed. In this example, we say a number is a prime by trying all numbers smaller than the square root of the number (but we use count*count &lt;= prime instead of count &lt;= sqrt(prime) because multiplying is more CPU friendly than calculating a square root. The % operator is used to take the modulo. Meaning that 7%2=1 because the remainder of the division of 7 by 2 is 1 (7-2*3=1). Within the main loop, you make some changes which impact the loop condition. Failing to do this will result in an eternal loop.</p>
<p>A second loop is seen on line 47 to 57; this is a for loop and has the following syntax:</p>
<p>如 果表达式1成立，语句1将被执行，否则表达式2将被检查；如果表达式是成立的，语句2将被执行，并且，如果所有的都不成立，语句三就会被执行。 else if和else部分都是可选的，你也可以增加更多的else if部分。一个条件会被认为是真当它在不为0的时候——它解释了第49行的代码</p>
<p>if else的特殊形式在第27行。这种形式不是那么常见，并且是典型的用于非常简洁的事物。这里，是一个简洁的说明函数应该返回0如果值是一个参数或者除数或者是1，否则的话。</p>
<p>第 一个循环是一个while循环，例如23到26行。这里，只要条件成立循环的部分将被执行，这个意味着它是潜在不被执行的。在这个例子当中，我们说一个数 字是一个质数，通过试计算所有比那个数小的平方根（但是我们用count*count &lt;= prime instead of count &amp; lt;= sqrt(prime) 因为处理器对乘法比计算平方根更友好。 百分号运算符用于计算模。7%2=1 因为以7为被除数2为除数的余数是 1(7-2*3=1)。不超出主循环，你做一些改变，并作用于循环条件。不这么做的话会造成一个死循环。</p>
<br />