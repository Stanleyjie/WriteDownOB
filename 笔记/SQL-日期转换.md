在SQL Server中，可以使用CONVERT()函数或FORMAT()函数将日期转换为yyyy-mm-dd格式。

使用CONVERT()函数：
```SQL
SELECT CONVERT(varchar, GETDATE(), 23) AS FormattedDate
```

使用FORMAT()函数（SQL Server 2012及更高版本）：
```SQL
SELECT FORMAT(GETDATE(), 'yyyy-MM-dd') AS FormattedDate
```

FORMAT()函数提供比CONVERT()更多的灵活性和选项，但是CONVERT()可能在性能上有微小的优势。选择使用哪种方法应基于特定的需求和数据库版本。