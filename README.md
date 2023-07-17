#总结<br>
1.collection接口：list；vector,arrlist,linklist（有序，可重复）<br>
                  set：hashset,treeset（有序，不可重复）<br>
2.map接口：hashmap，linkhashmap（无序，不可重复）<br>
3.常见异常类型：空指针异常（NullPointException），数组越界异常（ArrayIndexOutOfBoundsException<br>
），强制类型转换异常（ClassCastException），数字格式化异常（NumberFormatException），输入类型不<br>
匹配异常（InputMismatchException），算数运算符异常（ArithmeticException）：索引越界异常（Index<br>
OutOfBoundsException），SQL异常（SQLException），内存溢出异常（OutOfMemoryError）IO异常（IOEx<br>
ception），找不到文件异常（FileNotFoundException）<br>
4.异常处理方法：try-catch，throws，throw
5.throw，与throws的区别：throws放在方法声明的后面，表示报出异常，由该方法的调用者来处理；throw作<br>
用在方法内部，后面跟着的是异常的对象
6.泛型：操作List的时候就可以通过泛型对我们集合内的值进行规范和约束（不能在类中定义泛型参数化的静态属性，
不能创建类型参数的实类，泛型的类型参数不能是类型，不能创建泛型的异常类）
7.java 中泛型标记符
E - Element (在集合中使用，因为集合中存放的是元素)
T - Type（Java 类）
K - Key（键）
V - Value（值）
N - Number（数值类型）
？ - 表示不确定的 java 类型
8.上界通配符 < ? extends E>：用 extends 关键字声明，表示参数化的类型可能是所指定的类型，或者是此类型的子类。
9.下界通配符 < ? super E>： 用 super 进行声明，表示参数化的类型可能是所指定的类型，或者是此类型的父类型，直至 Object
10。线程与进程的区别：进程是程序的一次执行，进程是资源（CPU、内存等）分配的基本单位，它是程序执行时的一个实例。
线程是 CPU 的基本调度单位，是进程的一个执行流。
11.创建线程的几种方式
继承Thread类	编程比较简单	扩展性差
实现Runnable接口	扩展性强	相对复杂，没有返回结果
实现Callable+FutureTask接口	扩展性强，可得到结果	编程复杂
12.线程池：使用ExecutorService（接口）的实现类：TreadPollExecutor 自创建一个线程池对象
int corePoolSize：核心线程数
int maximumPoolSize：最大创建线程数
long keepAliveTime：存活时间
TimeUnit unit：Time类管理工具
BlockingQueue<Runnable> workQueue：指定阻塞队列
ThreadFactory threadFactory：线程工厂
RejectedExecutionHandler handler：拒绝策略
