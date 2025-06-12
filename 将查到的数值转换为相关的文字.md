```SQL
SELECT (case 
when Nature = 0 then '未定级'
when Nature = 1 then '一级医院'
when Nature = 2 then '二级医院' 
when Nature = 3 then '三级医院'
when Nature = 4 then '民营医院'
when Nature = 5 then '无等级'
end)as n1, * FROM Hospital
```