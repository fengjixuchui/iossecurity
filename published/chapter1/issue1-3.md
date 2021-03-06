
对iOS应用进行逆向分析的方法可以大致分为两类：

  * 静态分析（static analyze）
  * 动态分析（dynamic analyze）

###静态分析
顾名思义，静态分析法是在不执行iOS应用的情形下，对应用进行静态分析的一种方法。比如获取应用的文件系统结构，本地文件的分析、使用反汇编工具（Disassembler，比如IDA）查看内部代码，分析代码结构也是静态分析。

###动态分析
动态分析法是在iOS应用的执行过程中进行动态分析的一种方法，通过调试来分析代码，获得内存的状态等等。通过动态分析法，可以在观察应用的文件、网络等。动态分析中还常使用调试器（Debugger，比如gdb）分析应用的内部结构与原理。甚至可以使用工具（比如Cycript，后面会详细介绍该工具）动态修改内存，给内存打补丁。

在进行iOS逆向工程的时候，建议两种方法都采用，通常是先静态分析下收集应用的相关信息，然后使用动态分析获得进一步的信息。灵活的使用这两种方法，可以大大提供分析效率。


***
[#1 iOS逆向工程简介下的更多文章](http://security.ios-wiki.com/issue-1/)
