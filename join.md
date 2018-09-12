# homework 0912

###代码如下:
``` 
select p.cityName 省,s.cityName 市,null from s_provinces x
	join s_provinces s on x.parentId = s.id
	join s_provinces p on s.parentId = p.id
	where p.cityName = '广东省'
union 
select p.cityName 省,s.cityName 市,x.cityName 县 from s_provinces x
	join s_provinces s on x.parentId = s.id
	join s_provinces p on s.parentId = p.id
	where p.cityName = '广东省'
```
思路：

    1、先查找出所有的省和市，县（区）用空格占位
    2、查找出省、市、县（区）
    3、用 union 合并成一张表
    union:用于合并两个或多个select语句的结果集，并消除表中重复的行
            union 合并表，每个表必须有相等的字段数量，并且字段类型一一对应，
            每条列的顺序也要相同
