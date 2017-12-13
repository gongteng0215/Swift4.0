# **一段Swift的旅程** #

按照惯例，每学习一门新的程序语言，都在屏幕打印一下 **"Hello,world!"** 。在 **Swift** 中，只需要简单一行：

> print("Hello,world!")

如果你有写过 **C** 或者 **Objective-C** 的话，应该对这语法很熟悉。在 **Swift** 中，这行已经是一个完整的程序了，你不需要在导入一个单独的功能库，像输入/输出或者字符串处理之类的，像 **C** 就需要 `#include <stdio.h>` 和 `#include <string.h>` 。代码书写在全局范围都可以被作为程序的入口点，所以你也不需要一个 `main()` 函数。你也不需要在每一句代码声明的后面都加上;号。

这段旅程将通过给你足够的信息来告诉你怎么用**Swift**代码来完成多种多样的编程任务。别担心，如果你不能理解一部分代码，或者全部都不理解，那也没事，在本书的其他章节都会一一讲解。
    
    为了更好的体验，点击下面链接下载文件，并且用Xcode里的playground打开这一章节（Simple Values）。Playgrounds允许你编辑代码列
    表而且马上就能看到变化。

[Playgrounds下载](https://developer.apple.com/library/content/documentation/Swift/Conceptual/Swift_Programming_Language/GuidedTour.playground.zip)

## 简单的值 ##

用 `let` 声明常量，用 `var` 声明变量。常量的值在编译期间不需要被识别，但是你必须正确地给它赋一次值。这样表示你只要给常量赋过一次值之后，你在很多地方都可以用它。

>var myVariable = 42<br>
>myVariable = 50<br>
>let myConstant = 42<br>

一个常量的值的类型必须与你赋给它的值的类型一样。当然，你也没必要一直显式地声明它的类型。当你赋值一个常量或者变量的时候，只要给它一个值，让编辑器自己去推断值的类型。在上面的例子，编辑器推断出 `myVariable` 是一个整型，因为它初始化的值是一个整数。

如果初始化值不能提供足够的信息(或者根本没有初始化值)的话，在变量(常量)的后面加上 `:` 号和类型。

>let implicitInteger = 70<br>
>let implicitDouble = 70.0<br>
>let explicitDouble: Double = 70

    练习：
    创建一个常量，显式声明 Float 类型，并且赋值 4 。

值不会隐式地转化为另外一个类型。如果你需要把一个值转化为不同的类型，显式地创建一个所需类型的实例。

>let label = "The width is "<br>
>let width = 94<br>
>let widthLabel = label + String(width)

    练习：
    试着删除最后一行的 String 转换。你得到错误是什么？

还有一个更简单的方法在字符串里面包含值：把值写在括号 `()` 里面，然后在 `()` 前面加上 `\` 。举个例子：

>let apples = 3<br>
>let oranges = 5<br>
>let appleSummary = "I have \(apples) apples. "<br>
>let fruitSummary = "I have \(apples + oranges) pieces of fruit. "