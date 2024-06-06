### 1.LEFT ( character_expression , integer_expression )

函数说明：LEFT ( '源字符串' , '要截取最左边的字符数' )  
select LEFT('abcdefg',3);  
结果：abc

### 2.RIGHT ( character_expression , integer_expression )

函数说明：RIGHT ( '源字符串' , '要截取最右边的字符数' )，返回字符串中从右边开始指定个数的 integer_expression 字符  
select RIGHT('abcdefg',3);  
结果：efg

### 3.SUBSTRING ( expression , start , length )

函数说明：SUBSTRING ( '源字符串' , '截取起始位置(含该位置上的字符)' , '截取长度' )，返回字符、expression 表达式的一部分

select SUBSTRING('abcdefg',3 ,4);  //意思：从第三位开始截取，截取4位

结果：cdef

###  4.CHARINDEX(expression1, expression2 [,start_location])

函数说明：CHARINDEX 查询字符串所在的位置，expression1 为子字符串，expression2 为父字符串，start_location 表示开始位置。

select CHARINDEX('d', 'abcdef', 0);

结果：4