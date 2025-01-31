# 06 数据库表中记录的基本操作

DML: 增删改表中数据

1. 添加数据

```
insert into 表名(列名1， 列名2，..., 列名n) values(值1，值2，...,值n);
```

* 注意：
  1. 列名和值要一一对应。
  2. 如果表名后，不定义列名，则默认给所有列添加值。
  3. 除了数字类型，其他类型需要用引号（单、双引号）引起来

2. 删除数据

```
delete from 表名 where 条件;
truncate table 表名; -- 删除表，然后在创建一个一模一样的空表 
```

- 注意
  1. 如果不加条件，则删除表中所有记录。
  2. 如果腰删除所有记录
     1. `delete from 表名; --不推荐使用。有多少条记录就会执行多少次删除操作`  
     2. ` truncate table 表名; -- 推荐使用，效率更高 删除表，然后在创建一个一模一样的空表 `

2. 修改数据

```
update 表名 set 类名1 = 值1, 列名2 = 值2, ...,列名n = 值n, where 条件;
```

- 注意：
  - 如果不加任何条件，则会将表中所有记录全部修改。







































d