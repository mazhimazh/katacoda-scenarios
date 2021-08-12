在使用反射或动态代理等技术时，有时会导致频繁的类加载操作，进而会导致metaspace报OutOfMemoryError异常。下面使用class命令查看类是否频繁加载：

（1）运行`class`{{execute}} 命令，查看LoadedClassCount和UnloadedClassCount，如果LoadedClassCount属性的值一直在增长，而UnloadedClassCount属性的值几乎不增长，则基本可确认有频繁类加载操作；

（2）如果有类加载和卸载操作，会让metaspace在报出OutOfMemoryError之前，让committed的值慢慢逼近max的值。运行`metaspace`{{execute}} 命令，查看used和committed的值是否一直在增长，committed的值是否已经逼近了max的值。

