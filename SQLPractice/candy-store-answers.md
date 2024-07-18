# Answers

1. 
```sql
create table inventory (
  id number,
  name varchar(255),
  price number(4,2),
  description varchar(255),
  quantity number
);
```

2. 
```sql
insert into inventory values  (1001, 'Hershey Bar', 3.45, 'A small chocolate bar', 50);
insert into inventory values  (1002, 'Skittles', 3.05, 'A bag of rainbow colored candies', 100);
insert into inventory values  (2003, 'Gummy Bears', 5.55, 'A large bag of chewy fruit-flavored bears', 48);
insert into inventory values  (2005, 'Sour Gummy Worms', 9.55, 'A very large bag of gelatin worms', 20);
insert into inventory values  (3008, 'Lollipop', 2.25, 'A hard candy atop a stick', 268);
insert into inventory values  (9007, 'M&Ms', 1.95, 'A bag of small chocolate candies', 58);
```

3. 
```sql
select * from inventory;
```

4. 
```sql
update inventory set quantity=48 where id=1001;
```

5.
```sql
select description from inventory;
```

6. 
```sql
select name, price from inventory;
```

7. 
```sql
update inventory set description='A very large, delicious bag of worms' where id=2005;
```

8. 
```sql
update inventory set quantity=100 where id=9007;
```

9. 
```sql
update inventory set price=2.50 where id=3008;
```

10. 
```sql
select (price * quantity) from inventory where id=9007;
```

11.
```sql
select name, price from inventory where price = (select min(price) from inventory);
```


12.
```sql
select name, quantity from inventory where quantity = (select max(quantity) from inventory);
```

13.

The below is specific to Oracle 11g
```sql
select *  from (select * from inventory ORDER By price DESC) WHERE ROWNUM <= 3;
```

The below is specific to Oracle 12
```sql
select * from inventory ORDER BY price DESC FETCH FIRST 3 ROWS ONLY;
```

 