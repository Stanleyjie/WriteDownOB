假设现在有两张表，`Orders`和`Customers`，现在要更新`Orders`表中的`CustomerName`字段，将其设置为`Customers`表中对应的`CustomerName`。

```SQL
UPDATE o
SET o.CustomerName = c.CustomerName
FROM Orders o
INNER JOIN Customers c ON o.CustomerId = c.CustomerId
```

我们使用`INNER JOIN`来确保只有当两个表中都存在对应的客户ID时，才会进行更新。这样的操作确保了数据的一致性，并且避免了任何潜在的数据丢失。