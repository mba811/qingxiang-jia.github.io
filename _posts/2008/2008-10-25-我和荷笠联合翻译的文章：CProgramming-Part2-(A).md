---
layout: post
title: 我和荷笠联合翻译的文章：CProgramming-Part2 (A)
categories:
- Diandian
tags:
- Linux

---
<p>翻译：Lee <br />翻译状态：Working<br />校对：<br />校对状态：<br />二校：<br />二校状态：<br /></p>
<p>CProgramming-Part2</p>
<p>Flow Control</p>
<p>Flow control?</p>
<p>In the first article in this series, we learned to configure our system and compile and execute an application which didn't do anything useful at all, but we've got to start somewhere. This article is of major importance for novice programmers since here we'll introduce some thinking in code. This article will introduce functions, loops, and decision making, from a C perspective. But it should be clear that it's impossible to be complete in these short articles - the main goal of which is to create some base, and give people a starting point to continue their own journey.</p>
<p>流控制</p>
<p>流控制？</p>
<p>在这个系列的第一篇文章中，我们学习了怎样配置我们的系统，以及编译和执行一个完全没有可操作性的应用程序，但是我们已经开始步入正轨了。这篇文章主要针对的是编程初学者，因为我们将在代码中介绍一些思维。这篇文章将要用C语言的观点介绍函数、循环和决策。但是，应该指明的是，要想通过这三篇文章就学成是不可能的 —— 文章的主要目的是在读者的脑海里建立一些基础，给他们一个自己的C语言之旅的开端。</p>
<p>Functions</p>
<p>C is a so-called procedural language, which means that, when programming in C, you are working in a procedure-oriented way (the most popular alternative is object-oriented programming where people manipulate objects). So this means that when you need to solve a problem, you will start by breaking it up into smaller and reusable pieces. Suppose you were writing an office suite. You would have a print function to print your work on paper, and this function could be reused by all your suite components. In C most prototypes will look like:</p>
<p>return_type function_name(parameter_type1 param1, parameter_type2 param2)</p>
<p>Here you define a function called function_name, which returns a result of type return_type, and takes two parameters. If you don't have a return type, you would replace return_type by void. A more concrete example would look like:</p>
<p>int add(int a, int b){ return a+b; }</p>
<p>This adds two integers ('int a' says the the first variable is of type integer and that it is given the name 'a'), and returns their sum as an int. You could call it by putting 'add(1,1);' in your code. Note that the function needs to be defined before it gets used. And this is where the use of header files pop in; a header file will typically contain 'function prototypes'; this is the function header as displayed above, but terminated with a ';', and not followed by the function body. This is enough to let the C compiler know that a function, with a given signature, will be defined in the future, and let's just hope that the linker will find that function. In the example code, there are three functions defined. One is the main function, but there is also the function isPrime() defined on line 8 - which takes one integer as a parameter, and will return 0 when the integer is a prime. Then we have also printVersion() on line 34, which only prints some information, and doesn't return anything at all. printVersion() makes use of the symbols __DATE__ and __TIME__, which are replaced at compile time by the compilation timestamp. Other symbols such as __LINE__ and __FILE__ also exist - which can help during debugging. This function also uses the VERSION symbol which is defined on line 2. When the preprocessor is run (before the compiler), it does some plain string replaces; in this case VERSION will be replaced by '“1.0”'.</p>
<p>函数</p>
<p>C语言也叫做过结构化语言，意思是，当编写C的程序的时候，你在一个过程中工作 —— 面向过程（最流行的是面向对象的编程方式，在这种编程方式中，人们主要是操作对象）。所以，这个就意味着当你需要解决一个问题的时候，你要把它拆解成为更小的可重复利用的片段。假如你现在在编写一个办公套件。你可能有一个print函数来把你的内容显示在界面上，这个函数可能被你的其他组件重复利用。在C语言当中，大部分原型看起来是这样的：</p>
<p>return_type function_name(parameter_type1 param1, parameter_type2 param2)</p>
<p>这里，你定义了一个叫做function_name，它返回一个类return_type的结果，并带了两个参数。如果你没有一个循环类，你可以用void替换return_type。一个更具体的例子是：</p>
<p>int add(int a, int b){ return a+b; }</p>
<p>这个增加了两个整数（'int a' 意思是，第一个变量是整数的并且它被赋予名字'a'）并且返回它们的和作为一个整数。你可以叫它通过在你的代码中加入'add(1,1);'。注意，这个函数需要在用之前被定义。这就是头文件突然进来的作用。一个头文件将包括典型的'function prototypes'；这就是头文件在以上的显示，但是用一个“a”终止，不跟在函数部分的后面。这就足以让C的编译者知道那个函数，一个被给定的签名，将在以后被定义，让我们期望链接器可以发现那个函数。在示例代码中，有三个函数被定义。其中一个是主函数，但是也有一个isPrime()函数定义在第八行 —— 把整数看成是一个参数，并将返回0，当那个整数是质数的时候。然后我们也有printVersion() 在第34行，只是打印出一些信息，并不返回任何信息。printVersion() 利用符号__DATE__ and __TIME__，它将在编译的时候被编译时间戳替换。其他的符号像__LINE__ and __FILE__也存在，他们将在调试的时候起作用，这个函数也使用被定义在第二行的VERSION符号。当预处理程序被运行（在编译器之前），它完成一些字串替换；在这里VERSION被替换为“1.0”。</p>
<br />
<p><br /></p>