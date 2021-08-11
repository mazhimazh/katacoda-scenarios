
1.使用命令`use jstack_x@MAZHI`{{execute}} 来使用JStack_X插件。

2.使用`help`{{execute}} 获取jstack_x的详细使用帮助。  

3.使用`jps|grep demo.simulators.boot.ThreadSimulatorMain|split|attach`{{execute}} attach到simulator模拟程序

4.使用`lock -d -m`{{execute}} 检测死锁线程，其中的-d表示列出所有死锁的线程，-m表示显示尽量全面的信息。 根据列出的信息可知，模拟程序中发现了一个死锁。


