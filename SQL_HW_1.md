###1. ¬ывести все пол€ и все строки

####select * from qa_students_1;
____
###2. ¬ывести всех студентов в таблице

####select * from students;
____
###3. ¬ывести только Id пользователей

####select id from students;
____
###4. ¬ывести только им€ пользователей

####select name from students;
____
###5. ¬ывести только email пользователей

####select email from students;
____
###6. ¬ывести им€ и email пользователей

####select name,email from students;
____
###7. ¬ывести id, им€, email и дату создани€ пользователей

####select id,name,email,created_on from students;
____
###8. ¬ывести пользователей где password 12333

####select user from students,
####where password = '12333';
____
###9. ¬ывести пользователей которые были созданы 2021-03-26 00:00:00

####select user from students
####where created_on = '2021-03-26 00:00:00';
____
###10. ¬ывести пользователей где в имени есть слово јнна

####select user from students
####where name = 'јнна';
____
###11. ¬ывести пользователей где в имени в конце есть 8

####select user from students
####where name like '%8'
____
###12. ¬ывести пользователей где в имени в есть буква а

####select user from students
####where name like '%a%'
____
###13. ¬ывести пользователей которые были созданы 2021-07-12 00:00:00

####select user from students
####where created_on = '2021-07-12 00:00:00';
____
###14. ¬ывести пользователей которые были созданы 2021-07-12 00:00:00 и имеют пароль 1m313

####select user from students 
####where created_on = '2021-07-12 00:00:00' and password = '1m312';
____
###15. ¬ывести пользователей которые были созданы 2021-07-12 00:00:00 и у которых в имени есть слово Andrey

####select user from students
####where created_on = '2021-07-12 00:00:00' and name = 'Andrey';
____
###16. ¬ывести пользователей которые были созданы 2021-07-12 00:00:00 и у которых в имени есть цифра 8

####select user from students
####where created_on = '2021-07-12 00:00:00' and name like '%8%';
____
###17. ¬ывести пользовател€ у которых id равен 110

####select user from students
####where id = '110';
____
###18. ¬ывести пользовател€ у которых id равен 153

####select user from students\ 
####where id = '153';
____
###19. ¬ывести пользовател€ у которых id больше 140

####select user from students
####where id > '140';
____
###20. ¬ывести пользовател€ у которых id меньше 130

####select user from students
####where id < '130';
____
###21. ¬ывести пользовател€ у которых id меньше 127 или больше 188

####select user from students
####where id < '127' or id > '188';
____
###22. ¬ывести пользовател€ у которых id меньше либо равно 137

####select user from students
####where id <= '137';
____
###23. ¬ывести пользовател€ у которых id больше либо равно 137

####select user from students
####where id >= '137';
____
###24. ¬ывести пользовател€ у которых id больше 180 но меньше 190

####select user from students 
####where id > '180' and  id < '190';

____
###26. ¬ывести пользователей где password равен 12333, 1m313, 123313

####select user from students 
####where password = '12333' or password = '1m313' or password = '123313';
____
###27. ¬ывести пользователей где created_on равен 2020-10-03 00:00:00, 2021-05-19 00:00:00, 2021-03-26 00:00:00

####select user from students
####where created_on = '2020-10-03 00:00:00' or created_on = '2021-05-19 00:00:00' or created_on = '2021-03-26 00:00:00';
____
###28. ¬ывести минимальный id

####select MIN(id) from students; 
____
###29. ¬ывести максимальный.

####select MAX(id) from students;

____
###30. ¬ывести id пользовател€, им€, дату создани€ пользовател€. ќтсортировать по пор€дку возрастани€ даты добавлени€ пользоватлел€.

####select id,name,created_on from students
####order by created_on asc;

____
###31. ¬ывести id пользовател€, им€, дату создани€ пользовател€. ќтсортировать по пор€дку убывани€ даты добавлени€ пользоватлел€.

####select id,name,created_on from students 
####order by created_on desc;
