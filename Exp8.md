# <center>Experiment No.8
### Perform the following Query 
### 1. Display all employees with their dept name. 
~~~sql
SELECT E.EMPNO, E.ENAME, D.DNAME
FROM EMPLOYEE E
JOIN DEPARTMENT D
ON E.DEPTNO = D.DEPTNO;
~~~
~~~sql
SELECT E.ENAME, D.DNAME
FROM EMPLOYEE E, DEPARTMENT D
WHERE E.DEPTNO = D.DEPTNO;
~~~
### 2. Display those employees whose manager names is jones, and also display their manager name. 
~~~sql
SELECT 
    E.ENAME AS EMPLOYEE,
    M.ENAME AS MANAGER
FROM EMPLOYEE E
JOIN EMPLOYEE M
ON E.MGR = M.EMPNO
WHERE M.ENAME = 'JONES';
~~~
~~~sql
SELECT A.ENAME AS EMPLOYEE_NAME, B.ENAME AS MANAGER_NAME
FROM EMPLOYEE A, EMPLOYEE B
WHERE A.MGR = B.EMPNO
AND B.ENAME = 'JONES';
~~~
### 3. Display employee name, his job, his dept name, his manager name, his grade and make out of an under department wise.
~~~sql

~~~
### 4. List out all the employees name, job, and salary grade and department name for everyone in the company except ‘clerk’. Sort on salary display the highest salary.
~~~sql

~~~
### 5. Display employee name, his job and his manager. Display also employees who are without manager. 
~~~sql

~~~
### 6. List the employee name, job, annual salary, deptno, dept name and grade who earn 36000 a year or who are not clerks. 
~~~sql

~~~
### 7. List ename, job, annual sal, deptno, dname and grade who earn 30000 per year and who are not clerks. 
~~~sql

~~~
### 8. List out all employees by name and number along with their manager’s name and number also display ‘no manager’ who has no manager. 
~~~sql

~~~
### 9. Select dept name, dept no and sum of sal 
~~~sql

~~~
### 10. Display employee number, name and location of the department in which he is working
~~~sql

~~~
### 11. Display employee name and department name for each employee. 
~~~sql

~~~
## NOTES
~~~SQL
1. A JOIN combines rows from two or more tables based on a related column.

Example:
EMPLOYEE.DEPTNO ↔ DEPARTMENT.DEPTNO

2. INNER JOIN
Returns matching rows only
Excludes NULL matches

LEFT JOIN
Returns all rows from left table + matching rows
Includes NULL values
~~~
