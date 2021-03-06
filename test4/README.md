# Oracle数据库第四次实验

姓名：陈小屿 学号：201810414207 班级：18级软件工程2班

## 实验目的

### 了解Oracle表和视图的概念，学习使用SQL语句Create Table创建表，学习Select语句插入，修改，删除以及查询数据，学习使用SQL语句创建视图，学习部分存储过程和触发器的使用。

## 实验场景

### 假设有一个生产某个产品的单位，单位接受网上订单进行产品的销售。通过实验模拟这个单位的部分信息：员工表，部门表，订单表，订单详单表。

## 实验内容

### 录入数据--本要求至少有1万个订单，每个订单至少有4个详单。至少有两个部门，每个部门至少有1个员工，其中只有一个人没有领导，一个领导至少有一个下属，并且它的下属是另一个人的领导（比如A领导B，B领导C）。

### 序列的应用--插入ORDERS和ORDER_DETAILS 两个表的数据时，主键ORDERS.ORDER_ID, ORDER_DETAILS.ID的值必须通过序列SEQ_ORDER_ID和SEQ_ORDER_ID取得，不能手工输入一个数字。

### 触发器的应用--维护ORDER_DETAILS的数据时（insert,delete,update）要同步更新ORDERS表订单应收货款ORDERS.Trade_Receivable的值。


## 实验步骤

### 删除表和序列，删除表的同时会一起删除主外键、触发器、程序包。

![](1.png)

### 创建表DEPARTMENTS

![](2.png)

### 创建表EMPLOYEES并授权

![](3.png)

### 创建表PRODUCTS并授权

![](4.png)

### 创建触发器Comment

![](5.png)

### 创建表ORDERS

![](6.png)

### 创建本地分区索引ORDERS_INDEX_DATE

![](7.png)

### 创建3个触发器

![](8.png)

![](9.png)

![](10.png)

### 插入数据

![](11.png)

### 创建SEQUENCE

![](12.png)

