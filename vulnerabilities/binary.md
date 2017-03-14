# Auditing Binaries

You’ve made it all the way down to the native layer, this is what software is after you pull off all the covers. The flavor of native code we’re going to focus on today is 32-bit Intel x86. Intel processors have been a powerful force in personal computing since the 80’s and currently predominate desktop and server market. Understanding this instruction set will give you some insight into how the programs you use every day operate as well as provide a reference point for when you encounter other instruction sets like ARM, MIPS, PowerPC and SPARC.

This module is about becoming familiar with the native layer and developing strategies for understanding, analyzing and interpreting native code. By the end of this module you should be capable of performing a “reverse compilation” -- going from assembly fragments to statements in higher level languages -- and, in the process, deriving meaning and programmer intent.

## Lecture

Learning x86 can appear daunting at first and requires some dedicated study to master. We recommend some reading below to simplify the life.  

* [x86 Assembly Guide](http://www.cs.virginia.edu/~evans/cs216/guides/x86.html)
* [Introduction to x86 Assembly](https://www.youtube.com/watch?v=qn1_dRjM6F0&list=PLPXsMt57rLthf58PFYE9gOAsuyvs7T5W9)

## Workshop

The following programs are both “binary bombs.” Reverse engineer the following linux programs to identify the series of inputs that will “defuse” the bomb. Each successive level of the bomb focuses on a different aspect of native code. For example, in the lab from CMU you will encounter different data structures \(linked lists, trees\) as well as how control flow structures \(switches, loops\) manifest in native code. While reversing these programs you may find it useful to keep track of your progress by transforming what you see into C or another high level language.

You should aim to solve at least eight stages between the two labs. The CMU bomb lab has a secret phase and the RPI bomb lab has a phase that involves memory corruption, can you find and solve them?

* [CMU Binary Bomb Lab](http://csapp.cs.cmu.edu/public/bomb.tar)
* [RPI Binary Bomb Lab](http://www.cs.rpi.edu/academics/courses/spring10/csci4971/rev2/bomb)

## Tools

The two essential tools for working with native code are the debugger and the disassembler. We recommend you become familiar with the industry standard disassembler: IDA Pro. IDA will divide code into discrete chunks corresponding to the functions defined in the program's source code. Each function is then further subdivided into "basic blocks" defined by instructions that alter control flow. This makes it easy to identify loops, conditionals, and other control flow constructs at a glance.

Debuggers allow you to interact with and examine the state of running code by setting breakpoints and examining memory and register contents. You may find this useful as a sanity check if you are not seeing the results you expect your input to produce but be alert, some programs employ anti-debugger techniques and can modify program behavior in the presence of a debugger. The GNU Debugger \(gdb\) is the standard debugger for most linux systems. gdb can be acquired through the package manager in your chosen linux distribution.

* [IDA Pro Demo](https://www.hex-rays.com/products/ida/support/download_demo.shtml)
* [gdb](http://www.sourceware.org/gdb/)

## 



