## Graded PAs

Q1. Write an SQL statement to find the team_id of the players who were born before the year '2003'..  
[Database: FLIS]

```

select team_id
from players
where dob<'2003-01-01'

```
***

Q2. Write an SQL statement to find the colors of the home-jersey and the away-jersey (jersey_home_color, jersey_away_color) used by the team: 'All Stars'.   
[Database: FLIS]

```

select jersey_home_color,jersey_away_color
from teams
where name='All Stars'

```
***

Q3. Write an SQL statement to find the player id and name of players from the team: 'Arawali'.  
[Database: FLIS] 

```

select p.player_id,p.name
from players p,teams t
where p.team_id=t.team_id
and t.name='Arawali'

```
***

Q4. Write an SQL statement to find the first names and the roll number (student_fname, roll_no) of students who belong to the department with department code as 'CS' and who were born after '2002-06-15'.   
[Database: LIS] 

```

select student_fname,roll_no
from students
where department_code='CS'
and dob > '2002-06-15'

```
***

Q5. Write an SQL statement to find the first names and the last names of faculty (faculty_fname, faculty_lname) who belong to the department:'Computer Science' and joined after '2015-03-03'.   
[Database: LIS]
```

select faculty_fname,faculty_lname
from faculty f, departments d
where f.department_code=d.department_code
and d.department_name='Computer Science' 
and doj > '2015-03-03'

```
