# MySQL

## 目录

[TOC]

## 语句

| 语句   | 作用       |                     |
| ------ | ---------- | ------------------- |
| Create | 创建语句   | [跳转](#create语句) |
| Use    | 选择数据库 | [跳转](#Use语句)    |



## 示例

### 一、创建数据库

```mysql
Create DataBase if not exists `baseName`
```

1. `Create`创建语句

2. `DataBase`创建类型是数据库

3. `if not exista`如果有就创建,没有就不创建

### 二、创建表

```mysql
Create Table if not exists `tableName`
```



## create语句

```mysql
Create `type` `name`
```

1. `Create`创建语句

2. `type`类型
   - `DataBase`数据库
   - `Table`表

### 创建表

```mysql
Create Table if not exists `tableName`(
`attribute` `type` `Keyword`,
`endKeyword`
);
```

1. `tableName`表名
2. `attribute`属性名
3. `type`属性类型
   - Char()
   - VarChar()
   - DateTime
   - `decimal(_len, _scale)`
     - `_len`长度
     - `_scale`小数位数
   - Date
4. `keyword`关键字
   - `not null`不能为空
   - `Primary key`主键
   - `Check()`
     - 限制范围
       - `_attribute Between _num1 and _num2`
     - 可以为空
       - `_attribute is null`
5. `endKeyword`结束关键字
   - `Primary Key(_attributes)`主键组
   - `ForEign Key(_attribute) References _tableName(_attribute)`外码

## Use语句

```mysql
Use `dataBaseName`
```

1. `Use`选择语句
2. `dataBaseName`数据库名字

## Insert语句

```mysql
Insert Into `tableName`(`attributes`)
Values(`vals`),
(`vals`)
```

1. `tableName`表名
2. `attributes`属性组
3. `vals`内容组

## Alter语句

```mysql
Alter Table `tableName` `keyword`
```

1. `keyword`

   - `add`添加
     - `Add _attribute _type`
   - `Modify Column`修改字段
     - `Modify Column _attribute _type`
   - `Drop Column`删除字段
     - `Drop Column _attribute`

## Drop语句

```mysql
Drop Table `tableName`
```



