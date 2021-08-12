下面使用class命令查看类是否频繁加载和卸载，在使用反射或动态代理等技术时，有时频繁的类加载和卸载会导致metaspace报OutOfMemoryError异常。

（1）运行`metaspace`{{execute}} 命令，查看已使用内存used的值是否已经逼近了max的值；


（2）运行`class`{{execute}} 命令，查看LoadedClassCount和UnloadedClassCount，如果数值非常大，则基本可确认有频繁类加载和卸载的操作。

