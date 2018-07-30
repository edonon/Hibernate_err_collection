**org.hibernate.PropertyAccessException: Null value was assigned to a property of**
```
实际数据的数据类型和表字段的数据类型调整成数据类型一样的即可。
INT、INTEGER 是 NUMBER 的受限子类型（只表示整数），相当于 NUMBER(38)。
表字段的数据类型为float，而数据为NULL，就是这样子数据类型不一致才会导致这个错误
```
