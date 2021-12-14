## 1)
create table mentor (mentor_id integer, mentor_name text)

create table company_drives (user_id integer, drives integer)

create table codekata (user_id integer, solved integer)

create table courses (course_id integer, course_name text)

create table course_activated (user_id integer, courses text)

create table users (id integer primary key, user_name text, mentor integer)

create table attendance (user_id integer, attendance_days integer)

create table tasks (user_id integer, completed integer)

create table topics (topic_id integer, content varchar(50))

## 2)

### Mentor Table values

insert into mentor values (1,"john")

insert into mentor values (2,"cena")

insert into mentor values (3,"lebron")

insert into mentor values (4,"james")

insert into mentor values (5,"corden")

![image](https://user-images.githubusercontent.com/77113035/146030408-546631a4-9e8a-4c33-89d7-b873a915fc94.png)

### company drive table values

insert into company_drives values (1, 20)

insert into company_drives values (2, 25)

insert into company_drives values (3, 35)

insert into company_drives values (4, 55)

insert into company_drives values (5, 65)

![image](https://user-images.githubusercontent.com/77113035/146030503-c5e686e8-5f17-4c6a-b50b-a5183dc39b82.png)

### codekat table values

insert into codekata values (1, 20)

insert into codekata values (2, 10)

insert into codekata values (3, 14)

insert into codekata values (4, 54)

insert into codekata values (5, 4)

![image](https://user-images.githubusercontent.com/77113035/146030558-40229422-b818-440e-9026-ed663a181ee9.png)

### courses table values

insert into courses values (1, "html")

insert into courses values (2, "css")

insert into courses values (3, "js")

insert into courses values (4, "react")

insert into courses values (5, "node")

![image](https://user-images.githubusercontent.com/77113035/146030595-0a6451dd-9470-4a91-b49a-0c473edb6027.png)

### courses activated table values

insert into course_activated values (1, 1)

insert into course_activated values (1, 2)

insert into course_activated values (2, 3)

insert into course_activated values (2, 2)

insert into course_activated values (3, 4)

insert into course_activated values (3, 5)

insert into course_activated values (4, 1)

insert into course_activated values (5, 5)

insert into course_activated values (5, 4)

insert into course_activated values (5, 3)

insert into course_activated values (1, 1)

![image](https://user-images.githubusercontent.com/77113035/146030921-edb56d76-a24f-4dd0-a9e5-9cad340aea1d.png)

### users table values

insert into users values (1, "kumar", 1)

insert into users values (2, "naveen", 2)

insert into users values (3, "rakesh", 3)

insert into users values (4, "prem", 5)

insert into users values (5, "lokesh", 5)

![image](https://user-images.githubusercontent.com/77113035/146030713-4c48bc87-3600-4449-9bfc-1a2e33ec7a06.png)

### attendance table values

insert into attendance values (1, 10)

insert into attendance values (2, 15)

insert into attendance values (3, 21)

insert into attendance values (4, 11)

insert into attendance values (5, 22)

![image](https://user-images.githubusercontent.com/77113035/146030756-cc786739-a35f-42a1-9335-cd67bc7fe974.png)

### tasks table values

insert into tasks values (1, 10)

insert into tasks values (2, 9)

insert into tasks values (3, 12)

insert into tasks values (4, 8)

insert into tasks values (5, 11)

![image](https://user-images.githubusercontent.com/77113035/146030810-d3fc9830-5750-4e6a-a203-203406eec329.png)

### topics table value

insert into topics values (1, "why react? whats its advantage?")

insert into topics values (2, "why node? how to build a server?")

insert into topics values (3, "useContext and lifecycle methods")

insert into topics values (4, "hooks in react")

insert into topics values (5, "async ..await function")

![image](https://user-images.githubusercontent.com/77113035/146030852-57f301b3-4524-4b8d-a9d9-dc8f94841c5e.png)

## 3)
SELECT user_name, solved FROM users inner join codekata on users.id = codekata.user_id

![image](https://user-images.githubusercontent.com/77113035/146031519-ad9722da-e5a3-4bfb-8c98-25077d256acc.png)

## 4)
SELECT user_name, drives FROM users inner join company_drives on users.id = company_drives.user_id

![image](https://user-images.githubusercontent.com/77113035/146031619-b028a443-0042-4261-b375-dc9604773e9b.png)


## 5)
SELECT course_name, count(course_name) FROM courses inner join course_activated on courses.course_id = course_activated.courses group by course_name
![image](https://user-images.githubusercontent.com/77113035/146031708-0187a154-b2be-43fc-a442-cf972cc3278c.png)

## 6)
select * from mentor

![image](https://user-images.githubusercontent.com/77113035/146031887-1eaa03d8-97a9-4202-b391-8087c620ecde.png)


## 7)
select mentor_name, count(user_name) from mentor inner join users on mentor.mentor_id = mentor group by mentor_name

![image](https://user-images.githubusercontent.com/77113035/146032002-d1cde26d-bdd0-44d8-8885-1bcb0387afe4.png)

