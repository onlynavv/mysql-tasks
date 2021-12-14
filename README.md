1)
create table mentor (mentor_id integer, mentor_name text)
create table company_drives (user_id integer, drives integer)
create table codekata (user_id integer, solved integer)
create table courses (course_id integer, course_name text)
create table course_activated (user_id integer, courses text)
create table users (id integer primary key, user_name text, mentor integer)
create table attendance (user_id integer, attendance_days integer)
create table tasks (user_id integer, completed integer)
create table topics (topic_id integer, content varchar(50))

2)
insert into mentor values (1,"john")
insert into mentor values (2,"cena")
insert into mentor values (3,"lebron")
insert into mentor values (4,"james")
insert into mentor values (5,"corden")


insert into company_drives values (1, 20)
insert into company_drives values (2, 25)
insert into company_drives values (3, 35)
insert into company_drives values (4, 55)
insert into company_drives values (5, 65)


insert into codekata values (1, 20)
insert into codekata values (2, 10)
insert into codekata values (3, 14)
insert into codekata values (4, 54)
insert into codekata values (5, 4)




insert into courses values (1, "html")
insert into courses values (2, "css")
insert into courses values (3, "js")
insert into courses values (4, "react")
insert into courses values (5, "node")


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










insert into users values (1, "kumar", 1)
insert into users values (2, "naveen", 2)
insert into users values (3, "rakesh", 3)
insert into users values (4, "prem", 5)
insert into users values (5, "lokesh", 5)

insert into attendance values (1, 10)
insert into attendance values (2, 15)
insert into attendance values (3, 21)
insert into attendance values (4, 11)
insert into attendance values (5, 22)

insert into tasks values (1, 10)
insert into tasks values (2, 9)
insert into tasks values (3, 12)
insert into tasks values (4, 8)
insert into tasks values (5, 11)

insert into topics values (1, "why react? whats its advantage?")
insert into topics values (2, "why node? how to build a server?")
insert into topics values (3, "useContext and lifecycle methods")
insert into topics values (4, "hooks in react")
insert into topics values (5, "async ..await function")

