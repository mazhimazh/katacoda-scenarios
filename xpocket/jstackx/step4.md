
1.运行`autocheck help`{{execute}} 命令查看autocheck帮助信息。

2.运行`autocheck -c 3 -i 5`{{execute}} 命令对线程信息进行动态采集，-c指定采集次数，这里指定为3次，每次采集的时间间隔由-i指定，这里指定的为5秒。

3.当有线程数不断上涨时，可能是线程泄漏，需要使用autocheck命令进行多次采集比对进行确认。