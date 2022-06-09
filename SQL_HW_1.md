###1. ������� ��� ���� � ��� ������

####select * from qa_students_1;
____
###2. ������� ���� ��������� � �������

####select * from students;
____
###3. ������� ������ Id �������������

####select id from students;
____
###4. ������� ������ ��� �������������

####select name from students;
____
###5. ������� ������ email �������������

####select email from students;
____
###6. ������� ��� � email �������������

####select name,email from students;
____
###7. ������� id, ���, email � ���� �������� �������������

####select id,name,email,created_on from students;
____
###8. ������� ������������� ��� password 12333

####select user from students,
####where password = '12333';
____
###9. ������� ������������� ������� ���� ������� 2021-03-26 00:00:00

####select user from students
####where created_on = '2021-03-26 00:00:00';
____
###10. ������� ������������� ��� � ����� ���� ����� ����

####select user from students
####where name = '����';
____
###11. ������� ������������� ��� � ����� � ����� ���� 8

####select user from students
####where name like '%8'
____
###12. ������� ������������� ��� � ����� � ���� ����� �

####select user from students
####where name like '%a%'
____
###13. ������� ������������� ������� ���� ������� 2021-07-12 00:00:00

####select user from students
####where created_on = '2021-07-12 00:00:00';
____
###14. ������� ������������� ������� ���� ������� 2021-07-12 00:00:00 � ����� ������ 1m313

####select user from students 
####where created_on = '2021-07-12 00:00:00' and password = '1m312';
____
###15. ������� ������������� ������� ���� ������� 2021-07-12 00:00:00 � � ������� � ����� ���� ����� Andrey

####select user from students
####where created_on = '2021-07-12 00:00:00' and name = 'Andrey';
____
###16. ������� ������������� ������� ���� ������� 2021-07-12 00:00:00 � � ������� � ����� ���� ����� 8

####select user from students
####where created_on = '2021-07-12 00:00:00' and name like '%8%';
____
###17. ������� ������������ � ������� id ����� 110

####select user from students
####where id = '110';
____
###18. ������� ������������ � ������� id ����� 153

####select user from students\ 
####where id = '153';
____
###19. ������� ������������ � ������� id ������ 140

####select user from students
####where id > '140';
____
###20. ������� ������������ � ������� id ������ 130

####select user from students
####where id < '130';
____
###21. ������� ������������ � ������� id ������ 127 ��� ������ 188

####select user from students
####where id < '127' or id > '188';
____
###22. ������� ������������ � ������� id ������ ���� ����� 137

####select user from students
####where id <= '137';
____
###23. ������� ������������ � ������� id ������ ���� ����� 137

####select user from students
####where id >= '137';
____
###24. ������� ������������ � ������� id ������ 180 �� ������ 190

####select user from students 
####where id > '180' and  id < '190';

____
###26. ������� ������������� ��� password ����� 12333, 1m313, 123313

####select user from students 
####where password = '12333' or password = '1m313' or password = '123313';
____
###27. ������� ������������� ��� created_on ����� 2020-10-03 00:00:00, 2021-05-19 00:00:00, 2021-03-26 00:00:00

####select user from students
####where created_on = '2020-10-03 00:00:00' or created_on = '2021-05-19 00:00:00' or created_on = '2021-03-26 00:00:00';
____
###28. ������� ����������� id

####select MIN(id) from students; 
____
###29. ������� ������������.

####select MAX(id) from students;

____
###30. ������� id ������������, ���, ���� �������� ������������. ������������� �� ������� ����������� ���� ���������� �������������.

####select id,name,created_on from students
####order by created_on asc;

____
###31. ������� id ������������, ���, ���� �������� ������������. ������������� �� ������� �������� ���� ���������� �������������.

####select id,name,created_on from students 
####order by created_on desc;
