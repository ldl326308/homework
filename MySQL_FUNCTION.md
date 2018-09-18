# MySQL function
* select date_add(now(),interval 20 day);
    date_add 函数，时间的计算，上述代码是在当前时间加上21天
    其中，day可以改为year、month等，顾明思议，year加的是年
    
* select datediff('2017-09-12',now());
    datediff 函数，计算两个日期之间相差的天数
    
*  select dayofmonth('2019-09-12'); 得到日期中的日数 12
*  select dayofweek('2019-12-03');  得到星期，星期天为1，星期一为2，以此类推        
* select dayofyear('2019-09-08'); 得到该时间为那年中的第几天
      
* select extract(year from '2018-09-03'); 得到该时间年份 2018    

* select last_day('2018-09-03'); 得到该日期月份的最后一天，这里得到30

* select minute('2018-09-01 10:09:01'); 得到该时间的分钟，这里得到9

* select month('2018-02-12'); 得到该时间的月份，这里得到2

* select concat('李','哈哈'); 字符串连接，得到“李哈哈”

* 字符串截取
 
    select substring('Java开发工程师',5); 这里得到“开发工程师”
    select substring('Java开发工程师',5,2); 这里得到“开发”
    
* select left('Java开发工程师',5); 从字符串左边开始截取，截取5个长度，得到“Java开”
* select right('Java开发工程师',5); 从字符串右边开始截取，截取5个长度，得到“开发工程师”

* select lower('YKKJKDSJFSKkksfsfs');将字符串转小写
* select upper('kkfdjskf'); 将字符串转大写
* select repeat('哈',3); 字符串复制，这里得到“哈哈哈”
    
* SELECT REPLACE('这个人，我在珠海见过他。', '我', '你');  字符串的替换，第一个参数：要替换的字符串，第二个参数：要替换的字符串，第三个参数，替换成的字符串。
这里得到“这个人，你在珠海见过他。”    
 
* select reverse('这个是字符串顺序颠倒'); 这里得到“倒颠序顺串符字是个这” 
 
* select space(5); 返回空格字符串，这里得到5个空格组成的字符串   
   
   
    