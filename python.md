# 内存数据

1. type
   1. number
      1. 整数
         1. 十进制：十进制数字
         2. 二进制：0b二进制数字
         3. 八进制：0o八进制数字
         4. 十六进制：0x十六进制数字
      2. 浮点
      3. 复数：实数+复数（3+2j）
   2. str
      1. 普通字符串
   3. bytes
      1. 字节串
   4. bool
   5. list：[值,值,值]
   6. tuple：(值,值,值)
   7. dict：{键:值,键:值,键:值}
   8. set：{值,值,值}
   9. class（自定义类）
      1.  自定义对象
2. NoneType
   1. None
3. 自定义元类（metaclass）
4. 函数

python中元类才是顶级数据类型。类是二级数据类型，实例对象是三级数据类型。我们常说的数据类型实际上都是二级数据类型，这和其他语言讲的数据类型都是一级数据类型有所区别。

python中任何类型都是址传递。可变数据类型：list，dict，set；不可变数据类型：numbe，sting，tuple。当可变数据类型改变数据时调用者变量的地址不变，引用该地址的其他变量数据也改变；不可变数据类型改变数据时调用者变量地址改变，引用该地址的其他变量数据不改变；这里的改变数据指的是调用内部方法，而不是赋值。