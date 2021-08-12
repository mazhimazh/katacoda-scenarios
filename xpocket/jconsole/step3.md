
1.使用命令`use jconsole@JDK`{{execute}} 来使用jconsole插件。

2.使用`jps|grep demo.simulators.boot.ThreadSimulatorMain|split|attach`{{execute}} attach到simulator模拟程序

3.使用`help`{{execute}} 获取jconsole的详细使用帮助。 通过帮助信息可以看到jconsole能够列出年轻代的eden、survivor空间、老年代old空间以及非堆空间code cache、metaspace的已使用内存大小和最大内存大小。





