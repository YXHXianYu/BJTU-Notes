# Operating System

> 张迪
>
> dizhang@bjtu.edu.cn

## 0. Course Overview

* 课程安排
  * 双周周五实验课
  * 答疑：Thu 12:00-14:00, YF West 708

* Learning Objectives
  * OS concepts and algorithms
  * 对现实的OS有深入的理解

* Grading
  * Homework and class quiz: 20%
  * Experiments: 30%
    * Create an OS using Rust
  * Final exam: 50%
    * close book
    * 编程题考 XinHaoLiang, 如何使用 XHL 来避免死锁
  * Bonus points
    * Extra homework
    * Experimental Project Innovation

## 1. Introduction

### 1.1 Basic Introduction

* Layers of a Computer System
  * Applications - Utilities - OS - Hardware

* What is an OS?
  * **No universally accepted** defination
  * One defination
    * a system software to manage hardware resources, control program running, improve man-machine interface and provide support for application software
  * Another defination
    * Resource Manager
      * each program gets time
      * each program gets space
      * decides between conflicting requests
    * Extended Machine + User Interface
      * hides the messy details
      * easier to use
      * executes user programs

* OS software classification
  * Shell: Command line interface
  * GUI: Graphical user interface
  * Kernel: The interior of the operating system

* Characteristics of an OS
  * Concurrency
  * Sharing
  * Virtualization
  * Asynchronization

* Why are we studying OS?

* How to learn OS?

* What OSes are there?
  * Microsoft OS: MS DOS, MS Windows 3.x, ...
    * DOS: Disk OS
  * UNIX: BSD, SRV4, OSF1, ...
  * Linux: Fedora, Ubuntu, Debian, Archlinux, ...
  * Embedded OS: WinCE, Symbian, uClinux, ...
    * 嵌入式操作系统
  * Moblie OS: Android, iOS, HarmonyOS, ...

### 1.2 History and Evolution of OS

* History Phase 1
  * Uni-programming & Multi-programming
    * **Multi-programming** (多道程序设计): During the idle wait time, we can run a third or more tasks.
    * 为了提高效率

* History Phase 2
  * Interactive time-sharing
    * **Time-sharing** (分时): cpu时间被分给多个用户，多个用户可以通过终端同时访问系统
    * Time-sharing is logical extension in which CPU switches

* History Phase 3
  * GUI

* Histroy Phase 4 (1989-)
  * Distributed Systems
  * Network

* History Phase 5 (1995-)
  * Mobile Systems

* How does an OS work
  * When a computer boots, it needs to run a first program: **the bootstrap program**
    * Typically stored in the read only memory (ROM)
    * Generally known as the **firmware** or **bootloader**
  * The bootstrap program initializes the Computer
    * Register content, device controller contents, etc.
  * It then locates and loads the **OS kernel** into memory
  * The kernel starts the first process (called "init" on Linux)
  * And then, nothing happends until an **event** occurs
    * OS开始等待某些事件的发生

* OS is running
  * load code to memory
  * memory protection
  * The kernel is NOT a running job
    * It's code that **resides in memory** and **is ready to be executed** at any moment (when some event occurs)

* A note on kernel size
  * **not use too much memory**
  * **no memory protection**

* Proteced instructions
  * A subset of instructions that only the OS can execute

* User mode vs Kernel mode
  * User mode 用户态: protected instructions cannot be executed
  * Kernel mode 内核态：all instructions can be executed
  * CPU中有一个 a protected control register，上面有一个 **status bit / mode bit (标记位/状态位)**，存当前状态

* OS events
  * The OS can be seen as a **huge event handler**
  * There are 2 kinds of events: **interrupts** and **traps**
    * interrupts: 中断通常由外部事件导致(硬件)
    * traps: 用户程序需要执行一些kernel mode才能执行的指令

* System calls 系统调用
  * A system call is a special kind of trap
