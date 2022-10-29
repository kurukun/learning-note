# DDL操作
## DDL数据库操作
1. show databases —— 展示已有的数据库
2. create database 数据库名 —— 创建新数据库
3. select database() —— 查看当前所在数据库
4. use 数据库名 —— 切换到某一数据库
5. drop 数据库名 —— 删除某一数据库
## DDL表操作
- show tables —— 查看当前数据库已有的表
- create table 表名 (字段 字段类型, 字段 字段类型) —— 创建一个表
- desc 表名 —— 查看该表的详细
- show create table 表名 —— 查看创建该表时的明细
- alter table 表名 add/modify/change/drop/rename to... —— 分别为增、改字段类型、改字段名和类型、删除某字段、修改表名
- drop table 表名 —— 删除该表
# DML操作
## DML插入操作
1. insert into 表名(列名) values(值) —— 在所选列中插入值
2. insert into 表名(列1,列2...) values(列1值1, 列2值1...),(列1值2,列2值2...) —— 在多个列中插入多行值的写法
3. 可以在values后面使用where来加入过滤条件 如 where id = 1
4. delete from 表名 where 条件 —— 删除条件选中的数据
5. update 表名 set 列名 = xx where 条件 —— 更新数据
# DQL操作
select 列名 from 表名 —— 展示选中的数据
使用 order by 可以对查询的结果进行排序，如：
> select * from user order by id asc —— 升序，asc或desc不写时默认为asc
> select * from user order by id desc —— 降序
