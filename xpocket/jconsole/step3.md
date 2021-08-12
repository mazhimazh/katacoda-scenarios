
1.使用命令`use jconsole@JDK`{{execute}} 来使用jconsole插件。

2.使用`jps|grep demo.simulators.boot.ThreadSimulatorMain|split|attach`{{execute}} attach到simulator模拟程序

3.使用`help`{{execute}} 获取jconsole的详细使用帮助。 通过帮助信息可以看到jconsole能够列出年轻代的eden、survivor空间、老年代old空间以及非堆空间code cache、metaspace的已使用内存大小和最大内存大小。

下面使用jconsole命令进行内存泄漏问题确认。

（1）运行`gc`{{execute}} 命令后，运行`memory`{{execute}} 命令，记录HeapMemoryUsage项的已使用内存used的值；

（2）等待1分钟或更长时间...

（3）再次运行`gc`{{execute}} 命令，然后再运行`memory`{{execute}} 命令，查看HeapMemoryUsage项的已使用内存used的值。

（4）多次执行（1）、（2）、（3）步骤，如果used值持续上涨，那可能有内存泄漏的风险，需要观察更长的时间来进一步确认。



