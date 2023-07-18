#总结<br>
1.collection接口：list；vector,arrlist,linklist（有序，可重复）<br>
                  set：hashset,treeset（有序，不可重复）<br>
2.map接口：hashmap，linkhashmap（无序，不可重复）<br>
3.常见异常类型：空指针异常（NullPointException），数组越界异常（ArrayIndexOutOfBoundsException<br>
），强制类型转换异常（ClassCastException），数字格式化异常（NumberFormatException），输入类型不<br>
匹配异常（InputMismatchException），算数运算符异常（ArithmeticException）：索引越界异常（Index<br>
OutOfBoundsException），SQL异常（SQLException），内存溢出异常（OutOfMemoryError）IO异常（IOEx<br>
ception），找不到文件异常（FileNotFoundException）<br>
4.异常处理方法：try-catch，throws，throw<br>
5.throw，与throws的区别：throws放在方法声明的后面，表示报出异常，由该方法的调用者来处理；throw作<br>
用在方法内部，后面跟着的是异常的对象<br>
6.泛型：操作List的时候就可以通过泛型对我们集合内的值进行规范和约束（不能在类中定义泛型参数化的静态属性，<br>
不能创建类型参数的实类，泛型的类型参数不能是类型，不能创建泛型的异常类）<br>
7.java 中泛型标记符<br>
E - Element (在集合中使用，因为集合中存放的是元素)<br>
T - Type（Java 类）<br>
K - Key（键）<br>
V - Value（值）<br>
N - Number（数值类型）<br>
？ - 表示不确定的 java 类型<br>
8.上界通配符 < ? extends E>：用 extends 关键字声明，表示参数化的类型可能是所指定的类型，或者是此类型的子类。<br>
9.下界通配符 < ? super E>： 用 super 进行声明，表示参数化的类型可能是所指定的类型，或者是此类型的父类型，直至 Object<br>
10。线程与进程的区别：进程是程序的一次执行，进程是资源（CPU、内存等）分配的基本单位，它是程序执行时的一个实例。<br>
线程是 CPU 的基本调度单位，是进程的一个执行流。<br>
11.创建线程的几种方式<br>
继承Thread类	编程比较简单	扩展性差<br>
实现Runnable接口	扩展性强	相对复杂，没有返回结果<br>
实现Callable+FutureTask接口	扩展性强，可得到结果	编程复杂<br>
12.线程池：使用ExecutorService（接口）的实现类：TreadPollExecutor 自创建一个线程池对象<br>
int corePoolSize：核心线程数<br>
int maximumPoolSize：最大创建线程数<br>
long keepAliveTime：存活时间<br>
TimeUnit unit：Time类管理工具<br>
BlockingQueue<Runnable> workQueue：指定阻塞队列<br>
ThreadFactory threadFactory：线程工厂<br>
RejectedExecutionHandler handler：拒绝策略<br>
13.线程安全问题：多个线程同时共共享一个资源，并对他进行修改
线程同步:加锁：让多个线程依次访问同一个资源
14:锁对象为任意的唯一对象，影响其线程的进行
规范上：使用共享资源作为锁对象，对于实例方法使用this作为锁对象，对于静态方法使用字节码（类名：class）对象作为锁对象


