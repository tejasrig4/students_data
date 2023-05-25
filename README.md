# students_data
create database student_data;
use student_data;
create table students(
grades varchar(200),
f_name text,
l_name text,
dob date,
parent_name varchar(200),
phone_num int,
address varchar(200),
city varchar(200),
english int,
hindi int,
maths int,
science int,
social int,
total int,
percentage varchar(200)
);
select * from students;
insert into students(
grades,f_name,l_name,dob,parent_name,phone_num,address,city,english,hindi,maths,science,social,total,percentage)
values
('grade-1','vijay', 'l','2000-05-11',"abc",123456,"aaaaaa","hyd",55,61,59,49,70,294,"58 %"),
("grade-2",'raj', 'k','2002-08-15', "bca",234561,"bbbbbb","bang",61,59,71,57,65,313,"62 %"),
('grade-3','ajay', 's','2007-02-18',"cab",345621,"cccccc","vijw",58,89,75,72,68,362,"72 %"),
('grade-4','sohel', 'p','2006-08-12',"ehg",456321,"dddddd","rjy",58,69,72,51,64,314,"72 %"),
('grade-5','jahith', 'a','2004-03-27',"kpf",564321,"eeeeee",'kdp',61,45,58,64,71,299,"59 %"),
('grade-6','sai',' g','2015-09-29',"pkl",654321,"ffffff",'nelor',71,75,59,62,75,342,"68 %"),
('grade-7','surya',' k','2011-04-20',"hfj",789456,"gggggg","palkl",45,48,61,52,56,262,"52 %"),
('grade-8','vivek','m','2007-08-14','lop',897564,"hhhhhh",'elur',58,57,61,52,61,289,"57 %");

insert into students(grades,f_name,l_name,dob,parent_name,phone_num,address,city)
values('new_student','shiva','h','2011-09-26',"rolexx",12345678,"ladhak","kkkkkk");

select * from students
where percentage>60;
select * from students
