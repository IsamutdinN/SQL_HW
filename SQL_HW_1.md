### 1. Вывести все поля и все строки
``` sql
 SELECT * FROM qa_students_1;
 ```
____

### 2. Вывести всех студентов в таблице
```SQL
SELECT * FROM students;
```
____
### 3. Вывести только Id пользователей

```SQL
SELECT id FROM students;
```

____
### 4. Вывести только имя пользователей

```sql
SELECT name FROM students;
```
____

### 5. Вывести только email пользователей

```SQL
 SELECT email FROM students;
```
___

### 6. Вывести имя и email пользователей

```SQL
SELECT name,email FROM students;
```
____

### 7. Вывести id, имя, email и дату создания пользователей

```SQL
SELECT id,name,email,created_on FROM students;
```
____

### 8. Вывести пользователей где password 12333

```SQL
SELECT user FROM students,
WHERE password = '12333';
```
____

### 9. Вывести пользователей которые были созданы 2021-03-26 00:00:00

```SQL
SELECT user FROM students
WHERE created_on = '2021-03-26 00:00:00';
```
____

### 10. Вывести пользователей где в имени есть слово Анна

```SQL
SELECT user FROM students
WHERE name = 'Анна';
```
____

### 11. Вывести пользователей где в имени в конце есть 8

```SQL
SELECT user FROM students
WHERE name LIKE '%8'
```
____

### 12. Вывести пользователей где в имени в есть буква а

```SQL
SELECT user FROM students
WHERE name LIKE '%a%'
```
____

### 13. Вывести пользователей которые были созданы 2021-07-12 00:00:00

```SQL
SELECT user FROM students
WHERE created_on = '2021-07-12 00:00:00';
```
____

### 14. Вывести пользователей которые были созданы 2021-07-12 00:00:00 и имеют пароль 1m313

```SQL
SELECT user FROM students 
WHERE created_on = '2021-07-12 00:00:00' AND
password = '1m312';
```
____

### 15. Вывести пользователей которые были созданы 2021-07-12 00:00:00 и у которых в имени есть слово Andrey

```SQL
SELECT user FROM students
WHERE created_on = '2021-07-12 00:00:00' AND
name = 'Andrey';
```
____

### 16. Вывести пользователей которые были созданы 2021-07-12 00:00:00 и у которых в имени есть цифра 8

```SQL
SELECT user FROM students
WHERE created_on = '2021-07-12 00:00:00' AND 
name LIKE '%8%';
```
____

### 17. Вывести пользователя у которых id равен 110

```SQL
SELECT user FROM students
WHERE id = '110';
```
____

### 18. Вывести пользователя у которых id равен 153

```SQL
SELECT user FROM students
WHERE id = '153';
```
____

### 19. Вывести пользователя у которых id больше 140

```SQL
SELECT user FROM students
WHERE id > '140';
```
____

### 20. Вывести пользователя у которых id меньше 130

```SQL
SELECT user FROM students
WHERE id < '130';
```
____

### 21. Вывести пользователя у которых id меньше 127 или больше 188

```SQL
SELECT user FROM students
WHERE id < '127' OR id > '188';
```
____

### 22. Вывести пользователя у которых id меньше либо равно 137

```SQL
SELECT user FROM students
WHERE id <= '137';
```
____

### 23. Вывести пользователя у которых id больше либо равно 137

```SQL
SELECT user FROM students
WHERE id >= '137';
```
____

### 24. Вывести пользователя у которых id больше 180 но меньше 190

```SQL
SELECT user FROM students 
WHERE id > '180' AND  id < '190';
```
____

### 26. Вывести пользователей где password равен 12333, 1m313, 123313

```SQL
SELECT user FROM students 
WHERE password = '12333' OR password = '1m313'
OR password = '123313';
```
____

### 27. Вывести пользователей где created_on равен 2020-10-03 00:00:00, 2021-05-19 00:00:00, 2021-03-26 00:00:00

```SQL
SELECT user FROM students
WHERE created_on = '2020-10-03 00:00:00'
OR created_on = '2021-05-19 00:00:00'
OR created_on = '2021-03-26 00:00:00';
```
____

### 28. Вывести минимальный id

```SQL
SELECT MIN(id) FROM students; 
```
____

### 29. Вывести максимальный.

```SQL
SELECT MAX(id) FROM students;
```
____

### 30. Вывести id пользователя, имя, дату создания пользователя. Отсортировать по порядку возрастания даты добавления пользоватлеля.

```SQL
SELECT id,name,created_on FROM students
ORDER BY created_on ASC;
```
____

### 31. Вывести id пользователя, имя, дату создания пользователя. Отсортировать по порядку убывания даты добавления пользоватлеля.

```SQL
SELECT id,name,created_on FROM students 
ORDER BY created_on DESC;
```
