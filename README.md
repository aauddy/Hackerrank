Problem: THE PADS 
Link:https://www.hackerrank.com/contests/simply-sql/challenges/the-pads

Solution:

(select concat(Name ,"(" , lefT(Occupation,1) , ")") as Nm
from Occupations)
union
(SELECT CONCAT("There are a total of ", COUNT(Occupation), concat(" ", lower(occupation), "s.")) as Nm
FROM OCCUPATIONS
GROUP BY Occupation
ORDER BY count(OCCUPATION),occupation)
order by Nm

