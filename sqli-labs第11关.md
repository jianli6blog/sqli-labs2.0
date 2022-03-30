title: sql-labs 11关

**Less-11** POST - Error Based - Single quotes- String (基于错误的POST型单引号字符型注入)

注入语句：admin' and 1=1 --+

![image-20220330101425259](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220330101425259.png)

这里不用密码也能登陆成功，所以判断是POST形式的单引号字符型注入

![image-20220330101729185](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220330101729185.png)