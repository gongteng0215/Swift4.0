# **一段Swift的旅程** #

按照惯例，每学习一门新的程序语言，都应该在屏幕打印一下
**"Hello,world!"**。在**Swift**中，只需要简单一行：

> print("Hello,world!")

如果你有写过**C**或者**Objective-C**的话，应该对这语法很熟悉。在**Swift**中，这行已经是一个完成的程序了，你不需要在导入一个单独的功能库，像输入/输出或者字符串处理之类的，C需要 `#include <stdio.h>` 和 `#include <string.h>` 。代码书写在全局范围都可以被作为程序的入口点，所以你也不需要一个 `main()` 函数。你也不需要在每一句代码声明的后面都加上;号。

这段旅程将通过给你足够的信息来告诉你怎么用**Swift**代码来完成多种多样的编程任务。别担心，如果你不能理解一部分代码，或者全部都不理解，那也没事，在本书的其他章节都会一一讲解。

    备注：
    为了更好的体验，点击[这个链接](https://developer.apple.com/library/content/documentation/Swift/Conceptual/Swift_Programming_Language/GuidedTour.playground.zip)下载文件，并且用Xcode里的playground打开这一章节（Simple Values.xcplaygroundpage）。Playgrounds允许你编辑代码列表而且马上就能看到变化。

## 简单的值 ##

用 `let` 声明常量，用 `var` 声明变量。常量的值在编译期间不需要被识别，但是你必须正确地给它赋一次值。这样表示你只要给常量赋过一次值之后，你在很多地方都可以用它。
>var myVariable = 42<br>
>myVariable = 50<br>
>let myConstant = 42<br>

