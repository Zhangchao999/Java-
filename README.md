# Java虚拟机
Java的内存管理机制，虚拟机执行子系统，程序编译与代码优化，高效并发。

-----
TOP



-----

### Java内存管理机制

![java内存](https://github.com/Zhangchao999/Java-1/raw/master/pictures/1.jpg)
<br>图1

![java内存](https://github.com/Zhangchao999/Java-1/raw/master/pictures/2.jpg)
<br>图2

<br>
讲解:<br>
从线程的私有还是共享来说：<br>
	线程私有:程序计数器、Java虚拟机栈、本地方法栈。<br>
	线程共享:Java堆、方法区。<br>
	1、程序计数器:<br>
		>程序计数器是当前线程所执行的字节码的行号指示器。当CPU要执行指令时，需要从程序计数器中获得指令所存储单元的地址，再得到指令。<br>
		>由于再任意时刻，一个CPU只能执行一条线程中的指令，因此，为了使每个线程在线程执行后回到原来的线程所执行的位置，所以，每个线程都需要单独的程序计数器。<br>
	2、Java虚拟栈:<br>
		>Java栈中存放的是一个个的栈帧，每个栈帧对应的是一个被调用的方法，在栈帧中包括:局部变量表，操作数栈，运行时常量池，方法的返回地址，附加信息。<br>
	3、本地方法栈:<br>






