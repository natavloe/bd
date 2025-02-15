# bd
bd al
1) Выберите из таблицы orders все заказы

SELECT * FROM orders 

![image](https://github.com/user-attachments/assets/61dbf111-7530-40c4-b802-3a12d1a4cd43)


2) Выберите из таблицы orders все заказы кроме новых. У новых заказов status равен "new". Использовать in

   SELECT * FROM orders WHERE STATUS IN ('cancelled','in_progress','delivery')

![image](https://github.com/user-attachments/assets/7f06d14d-7898-40ad-beda-266c7019d9a0)

3) Выберите из таблицы orders все новые и отмененные заказы. У отмененных заказов status равен "cancelled". У новых заказов status равен "new".

   SELECT * FROM orders WHERE STATUS IN ('cancelled','new')

![image](https://github.com/user-attachments/assets/16599c87-b5a9-4d75-97f9-16c9f481a3f3)

4) Выберите из таблицы orders все заказы содержащие более 3 товаров (products_count).
Вывести нужно только номер (id) и сумму (sum) заказа.

SELECT id,SUM FROM orders WHERE products_count > 3

![image](https://github.com/user-attachments/assets/c898ea57-71a9-4a87-bc6c-c47fb1e305af)
