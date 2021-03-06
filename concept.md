### 对一些关键概念的理解

1. javascript是单线程的，浏览器是多线程的

> javascript 是单线程的

JS运行在浏览器中，是单线程的，每个window一个JS线程，既然是单线程的，在某个特定的时刻只有特定的代码能够被执行，并阻塞其它的代码。而浏览器是事件驱动的（Event driven），
浏览器中很多行为是异步（Asynchronized）的，会创建事件并放入执行队列中。javascript引擎是单线程处理它的任务队列。所以当多个事件触发时，会依次放入队列，
然后一个一个响应。

> 浏览器是多线程的

虽然JS运行在浏览器中，是单线程的，但浏览器不是单线程的。浏览器中很多异步行为都是由浏览器新开一个线程去完成。javascript引擎线程是浏览器多个线程中的一个，
它本身是单线程的。浏览器还包括很多其他线程，如界面渲染线程，浏览器事件触发线程，Http请求线程等。

**************************************************

2. 进程与线程的区别与联系

* Reference 
1. [进程和线程的区别与联系](https://blog.csdn.net/u012349696/article/details/50914155)
2. [线程和进程的区别是什么？](https://www.zhihu.com/question/25532384)

* 进程和线程都是一个时间段的描述，是CPU工作时间段的描述，只不过是颗粒大小的问题。

> 进程就是包括程序执行上下文切换的程序执行时间的总和，包括CPU加载程序执行上下文，CPU执行程序， 和CPU保存程序执行上下文。

> 程序的执行又可以细化为一个个线程，线程是进程的一部分，它没有自己的地址空间，线程共享进程的上下文环境，是更为细小的CPU时间段。


