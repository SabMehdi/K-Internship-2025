### **1. Explore the Schema**mysql> show tables;
+---------------------------+
| Tables_in_kinternship2025 |
+---------------------------+
| customers                 |
| order_items               |
| orders                    |
| payments                  |
| products                  |
+---------------------------+
describe customers
    -> ;
+-------------+--------------+------+-----+---------+-------+
| Field       | Type         | Null | Key | Default | Extra |
+-------------+--------------+------+-----+---------+-------+
| customer_id | varchar(255) | YES  |     | NULL    |       |
| first_name  | varchar(255) | YES  |     | NULL    |       |
| last_name   | varchar(255) | YES  |     | NULL    |       |
| email       | varchar(255) | YES  |     | NULL    |       |
| phone       | varchar(255) | YES  |     | NULL    |       |
| address     | varchar(255) | YES  |     | NULL    |       |
| city        | varchar(255) | YES  |     | NULL    |       |
| state       | varchar(255) | YES  |     | NULL    |       |
| postal_code | varchar(255) | YES  |     | NULL    |       |
| country     | varchar(255) | YES  |     | NULL    |       |
+-------------+--------------+------+-----+---------+-------+
mysql> describe order_items;
+------------+--------------+------+-----+---------+-------+
| Field      | Type         | Null | Key | Default | Extra |
+------------+--------------+------+-----+---------+-------+
| order_id   | varchar(255) | YES  |     | NULL    |       |
| product_id | varchar(255) | YES  |     | NULL    |       |
| quantity   | varchar(255) | YES  |     | NULL    |       |
| price      | varchar(255) | YES  |     | NULL    |       |
+------------+--------------+------+-----+---------+-------+

mysql> describe orders
    -> ;
+--------------+--------------+------+-----+---------+-------+
| Field        | Type         | Null | Key | Default | Extra |
+--------------+--------------+------+-----+---------+-------+
| order_id     | varchar(255) | YES  |     | NULL    |       |
| customer_id  | varchar(255) | YES  |     | NULL    |       |
| order_date   | varchar(255) | YES  |     | NULL    |       |
| status       | varchar(255) | YES  |     | NULL    |       |
| total_amount | varchar(255) | YES  |     | NULL    |       |
+--------------+--------------+------+-----+---------+-------+

mysql> describe payments; 
+----------------+--------------+------+-----+---------+-------+
| Field          | Type         | Null | Key | Default | Extra |
+----------------+--------------+------+-----+---------+-------+
| order_id       | varchar(255) | YES  |     | NULL    |       |
| payment_date   | varchar(255) | YES  |     | NULL    |       |
| amount         | varchar(255) | YES  |     | NULL    |       |
| payment_method | varchar(255) | YES  |     | NULL    |       |
| status         | varchar(255) | YES  |     | NULL    |       |
+----------------+--------------+------+-----+---------+-------+
5 rows in set (0.00 sec)
describe products;
+--------------+--------------+------+-----+---------+-------+
| Field        | Type         | Null | Key | Default | Extra |
+--------------+--------------+------+-----+---------+-------+
| product_id   | varchar(255) | YES  |     | NULL    |       |
| product_name | varchar(255) | YES  |     | NULL    |       |
| description  | varchar(255) | YES  |     | NULL    |       |
| price        | varchar(255) | YES  |     | NULL    |       |
| stock        | varchar(255) | YES  |     | NULL    |       |
| category_id  | varchar(255) | YES  |     | NULL    |       |
+--------------+--------------+------+-----+---------+-------+