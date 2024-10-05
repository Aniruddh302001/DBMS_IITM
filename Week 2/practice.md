## Practice PAs

Q1. Write a SQL statement to find the name of the manager of the team: 'All Stars'.  
[Database: FLIS]

```

Select m.name
from managers as m,teams as t
where m.team_id=t.team_id
and t.name='All Stars'

```
***

Q2. Write an SQL statement to find the names of all teams.  
[Database: FLIS]

```

select name from teams

```
***

Q3. Write an SQL statement to find the titles of books authored by an author having first name as 'Joh Paul' and last name as 'Mueller'.  
[Database: LIS] 

```

select title
from book_catalogue b_c,book_authors b_a
where b_c.isbn_no=b_a.isbn_no
and author_fname='Joh Paul'
and author_lname='Mueller'

```
***

Q4. Write a SQL statement to find the titles of books published by 'McGraw Hill Education'.  
[Database: LIS]

```

select title
from book_catalogue
where publisher='McGraw Hill Education'

```
***

Q5. Write a SQL statement to display the first name and the last name of students (student_fname, student_lname) pursuing 'PG' courses.  
[Database: LIS]

```

select student_fname,student_lname
from students s, members m
where s.roll_no=m.roll_no
and member_type='PG'

```
