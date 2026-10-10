# 任务要求： 
创建mysql服务器 

```sql
mysql> CREATE DATABASE mydb CHARACTER SET utf8mb4 COLLATE utf8mb4_unicode_ci;
Query OK, 1 row affected (0.01 sec)
mysql> CREATE USER 'myuser'@'localhost' IDENTIFIED BY '111111';
Query OK, 0 rows affected (0.02 sec)
mysql> GRANT ALL PRIVILEGES ON mydb.* TO 'myuser'@'localhost';
Query OK, 0 rows affected (0.01 sec)
mysql> FLUSH PRIVILEGES;
Query OK, 0 rows affected (0.00 sec)
mysql> SHOW DATABASES;
+--------------------+
| Database           |
+--------------------+
| information_schema |
| mydb               |
| mysql              |
| performance_schema |
| sys                |
+--------------------+
5 rows in set (0.00 sec)

mysql> exit
Bye
```
最后使用dbeaver-ce 连接数据库，效果如图 
![image](image/L3.png)