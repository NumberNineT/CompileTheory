
汇编原理基础知识:

将某一种语言编译成为可执行程序中间需要经过很多步骤:词法分析、语法分析、语义分析、构建语义抽象树、计算栈、等。

编译器的作用:生成汇编代码, 接下来的工作由汇编器来完成。
前端(语法分析) -> 后端(根据CPU(ARM架构、X86架构...)支持的指令集,转换合适的汇编指令)

也可以再加上代码优化的环节(中端)
前端 -> 中端(代码优化) -> 后端

eg:
(1)可以计算简单加法的栈式编译器，如:
n
e1+e2
等;

(2)为编译器添加代码优化的功能, eg:a=1+2+3, 可以直接优化为a=6, 在编译阶段(静态)就可以完成的计算; 

涉及到的知识:各种数据结构:树(后序遍历)、栈(push, pop)等，用 C 实现