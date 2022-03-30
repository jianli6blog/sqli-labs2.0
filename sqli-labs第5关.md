title: sql-labs 5关

Less-5 GET - Double Injection - Single Quotes - String (双注入GET单引号字符型注入/基于’字符型的错误回显注入)

![image-20220330092509735](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220330092509735.png)

看到这个报错信息，第一反应就是布尔型盲注、报错型注入、时间延迟型盲注了

下面给出验证时间延迟型的盲注：

http://45.32.113.109:40430/Less-5/?id=1' and sleep(5) --+

发现明显延迟，说明猜测正确。接下来的思路是通过延迟，依次爆破数据库长度，数据库名，表名，列名，以及字段。

![image-20220330093226023](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220330093226023.png)