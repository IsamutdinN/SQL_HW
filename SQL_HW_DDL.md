## Таблица employees

### Создать таблицу employees
### Наполнить таблицу employee 70 строками.

### create table employees ( 
###	id serial primary key,
###	employee_name varchar(50) not null
### );
 
***--2	Августин***
***--3	Авраам***
***--4	Аврора***

***...***

***--68	Лада***
***--69	Лариса***
***--70	Лев***

## Таблица salary

### Создать таблицу salary
### Наполнить таблицу salary 15 строками:
***- 1000***
***- 1100*** 

***...***




### create table salary (
### id serial primary key,
### monthly_salary varchar(50) not null
### );

### insert into salary(monthly_salary)
### values
***(1000),***
***(1100),***
***(1200),***

***...***

***(2300),***
***(2400),***
***(2500);***
 
## Таблица employee_salary

### Создать таблицу employee_salary
### Наполнить таблицу employee_salary 40 строками:
### - в 10 строк из 40 вставить несуществующие employee_id


### create table employee_salary### 
### (id serial primary key,
### employee_id int not null unique,
### salary_id  not null
### );

### insert into employee_salary (id, employee_id, salary_id)
### values
***(1, 2, 3),***
***(2, 3, 4),***
***(3, 4, 5),***

***...***

***(38, 39, 40),***
***(39, 40, 41),***
***(40, 41, 42);***

## Таблица roles

### Создать таблицу roles
### Поменять тип столба role_name с int на varchar(30)
### Наполнить таблицу roles 20 строками:

	
### create table roles (
### id serial primary key,
### role_name varchar(30) not null unique
### );

### insert into roles (id, role_name)
### values### 
***(1, 'Junior Python developer'),***
***(2, 'Middle Python developer'),***
***(3, 'Senior Python developer'),***
***(4, 'Junior Java developer'),***
***(5, 'Middle Java developer'),***
***(6, 'Senior Java developer'),***
***(7, 'Junior JavaScript developer'),***
***(8, 'Middle JavaScript developer'),***
***(9, 'Senior JavaScript developer'),***
***(10, 'Junior Manual QA engineer'),***
***(11, 'Middle Manual QA engineer'),***
***(12, 'Senior Manual QA engineer'),***
***(13, 'Project Manager'),***
***(14, 'Designer'),***
***(15, 'HR'),***
***(16, 'CEO'),***
***(17, 'Sales manage'),***
***(18, 'Junior Automation QA engineer'),***
***(19, 'Middle Automation QA engineer'),***
***(20, 'Senior Automation QA engineer');***
 
## Таблица roles_employee

### Создать таблицу roles_employee
### Наполнить таблицу roles_employee 40 строками:

### create table roles_employee(id serial not null unique foreign key employees(id),
### role_id int not null foreign key roles(id)
### ); 

### insert into roles_employee (id, employee_id, salary_id)
### values
***(1, 2, 3),***
***(2, 3, 4),***
***(3, 4, 5),***

***...***

***(38, 39, 40),***
***(39, 40, 41),***
***(40, 41, 42);***

