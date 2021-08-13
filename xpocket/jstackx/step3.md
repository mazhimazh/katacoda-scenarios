
1.使用命令`use jstack_x@MAZHI`{{execute}} 来使用JStack_X插件。

2.使用`help`{{execute}} 获取jstack_x的详细使用帮助。  

3.使用`jps|grep com.classloading.Bootstrap|split|attach`{{execute}} attach到simulator模拟程序。

4.运行`autocheck`{{execute}} 命令，这个命令会自动检测死锁、锁竞争激烈、线程数不断上涨等情况。

5.使用`lock -d -m`{{execute}} 继续查看死锁线程的详细信息，其中的-d表示列出所有死锁的线程，-m表示显示尽量全面的信息。

6.当有锁的激烈竞争时，可使用 lock -m -f address 命令查看某个锁的具体信息。


