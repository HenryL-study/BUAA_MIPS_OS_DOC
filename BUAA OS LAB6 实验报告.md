#### BUAA OS LAB6 实验报告

##### Thinking 6.1

把父子进程所拥有的文件描述法互换即可，即把父子进程中fildes的 0换成1，,换成0

##### Thinking 6.2

这个dup函数我没有看出来。感觉这个函数是用来把一个文件描述符里的内容拷贝到一个新的文件描述符中，实在没找出由于这种不同步修改pp_ref 而导致的进程竞争问题。

##### Thinking 6.3

在我们的操作系统中，进行系统调用会陷入内核态并且关中断，这导致必须要把完整的系统调用代码执行完才会返回用户态。所以进行系统调用一定是原子操作。但是如果一个操作系统中允许多重中断的话就不一定了。

##### Thinking 6.4

1. 可以解决上述的竞争问题。因为如果先解除fd的映射的话，可以让pageref(p[])先减一，保证了pageref(p[]) <= pageref(pipe)这个等式一定成立，所以不会出现竞争问题。
2. 由于对于dup的理解不是很深刻，这个也没有看出来，所以没有解决。