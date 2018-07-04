/_ create table person(
id integer primary key autoincrement,
name varchar(35),
age integer,
height integer,
city varchar(40),
favoritecolor varchar(20)
) _/

/_ insert into person(name,age,height,city,favoritecolor)
values
('Sam',90,170,'Villa','purple'),
('Rebe',17,160,'Shank','pink'),
('Tim',7,95,'Jilly','blue'),
('Bob',12,120,'AppleTown','yellow'),
('Toe',23,200,'RepoCity','green') _/

/_ select _ from person order by height desc _/
/_ select _ from person order by height asc _/
/_ select _ from person order by age desc _/
/_ select _ from person where age > 20 _/
/_ select _ from person where age = 18 _/
/_ select _ from person where age < 20 or age > 30 _/
/_ select _ from person where age != 27 _/
/_ select _ from person where favoritecolor != 'red' _/
/_ select _ from person where favoritecolor != 'red' and favoritecolor !='blue' _/
/_ select _ from person where favoritecolor = 'orange' or favoritecolor ='green' _/
/_ select _ from person where favoritecolor in ('orange','green','blue') _/
/_ select _ from person where favoritecolor in ('yellow','purple') _/

/_ create table orders(
PersonID integer primary key autoincrement,
ProductName varchar(35),
ProductPrice float,
Quantity integer
) _/

/_ insert into orders(productname,productprice,quantity)
values
('Cheese',20,170),
('Fruit',5,160),
('Juice',7,95),
('Meat',12,120),
('Potato',80,200) _/

/_ select _ from orders _/
/_ select sum(quantity) from orders _/
/_ select sum(productprice) from orders _/
/_ select sum(productprice*quantity) from orders where personid = 4 */

/_ insert into artist(name)
values
('Jim'),
('Kim'),
('Bob') _/

/_ select _ from artist order by name desc limit 10 _/
/_ select _ from artist order by name asc limit 5 _/
/_ select _ from artist where name like "black%" _/
/_ select _ from artist where name like "%black%" _/

/_ select firstname,lastname from employee where city = "Calgary" _/
/_ select firstname,lastname,MAX(birthdate) from employee _/
/_ select firstname,lastname,MIN(birthdate) from employee _/
/_ select _ from employee where reportsto = 2 _/
/_ select count(_) from employee where city LIKE "lethbridge" _/

/_ select count(_) from invoice where billingcountry like 'usa' _/
/_ select MAX(total) from invoice _/
/_ select MIN(total) from invoice _/
/_ select _ from invoice where total > 5 _/
/_ select count(_) from invoice where total < 5 _/
/_ select _ from invoice where billingstate in ("CA","TX","AZ") _/
/_ select avg(total) from invoice _/
/_ select sum(total) from invoice _/
