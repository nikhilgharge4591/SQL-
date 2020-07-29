# HackerRank SQL-

Basic SQL SELECT Query Questions:

select * from CITY where POPULATION > 100000 AND COUNTRYCODE = "USA"


SQL Solutions from HackerRank

BST Problem -

SELECT DISTINCT N, 
CASE WHEN N NOT IN (SELECT DISTINCT P FROM BST WHERE P IS NOT NULL)
     THEN "Leaf"
     WHEN P IS NULL THEN "Root"
     ELSE "Inner"
     END AS P
FROM BST
ORDER BY N


HIGHER THAN 75

SELECT NAME FROM STUDENTS WHERE MARKS > 75 ORDER BY RIGHT(NAME, 3), ID ASC

ISOSCELES TRIANGLE

SELECT CASE 
           WHEN A + B > C AND B + C > A AND A + C > B THEN
               CASE
                   WHEN A = B AND B = C THEN 'Equilateral'
                   WHEN A = B OR B = C OR A = C THEN 'Isosceles'
                   ELSE 'Scalene'
               END
           ELSE 'Not A Triangle'
         END
FROM TRIANGLES
