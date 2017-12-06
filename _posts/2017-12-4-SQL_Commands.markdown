---
layout: post
title:  "SQL Review"
date:   2017-12-04 23:24:08 -0400
categories: study
---

**SELECT:** 

	SELECT * 
	FROM TABLE;

**DISTINCT:** 

	SELECT DISTINCT * 
	FROM TABLE;

**WHERE:** 

	SELECT *
	FROM TABLE
	WHERE CONDITION;

**AND, OR NOT**

	:)

**ORDER BY:**

	SELECT *
	FROM TABLE
	WHERE CONDITION
	ORDER BY TABLE.COL ASC|DESC;

**INSERT INTO:**

	INSERT INTO TABLE_NAME(COL1,COL2)
	VALUES(V1,V2)
	------------- OR
	INSERT INTO TABLE_NAME(V1,V2)

**UPDATE:**

	UPDATE TABLE
	SET COL1 = V1,COL2 = V2
	WHERE CONDITION;

**DELETE:**

	DELETE FROM TABLE_NAME
	WHERE CONDITION

**MIN/MAX:**

	SELECT (COL1,COL2) MIN/MAX(COL1)
	FROM TABLE;
	(GROUP BY COL1 COL2 COL3)
	**Group by need to contain all (or more) cols in select, Same rules applies to all**
	**aggregate functions (MIN, MAX, COUNT, AVG, SUM)**
	**In oracle sql, if col1,col2,aggfun_return is what we want, but we also need col3 adding**
	**col3 to group by/select might result in unique(col1,col2,col3,aggfun_return) but**
	**duplicate(col1,col2,aggfun_return)**

**COUNT/AVG/SUM**

	SELECT COUNT(COL)
	FROM TABLE;

	SELECT AVG(COL)
	FROM TABLE;

	SELECT SUM(COL)
	FROM TABLE;

**LIKE**
	
	SELECT *
	FROM TALBE
	WHERE COL LIKE "%_"; % match 0-n/ _ match exactly 1

**IN**
	
	SELECT *
	FROM TALBE
	WHERE COL IN (V1,V2,...)

# **JOINS**

	**INNER JOIN** Returns A & B
	SELECT *
	FROM TABLE A
	INNER JOIN TABLE B
	ON CONDITION;

	**FULL JOIN** Returns A OR B
	SELECT *
	FROM TABLE A
	FULL JOIN TABLE B
	ON CONDITION;

	**LEFT JOIN** Returns A + A & B
	SELECT *
	FROM TABLE A
	LEFT JOIN TABLE B
	ON CONDITION;

	**RIGHT JOIN** Returns B + A & B
	SELECT *
	FROM TABLE A
	RIGHT JOIN TABLE B
	ON CONDITION;

**DIFFERENCE BETWEEN JOINS & UNION**
	
	JOINS can have different cols, when join need condition, empty
	data is NULL.
	UNION must have same cols, no need condtion, just combine 
	results from Table A followed by Table B with the col name
	definded in A.

**UNION**
	
	SELECT COL1,COL2
	FROM TABLE A
	UNION
	SELECT COL1,COL2
	FROM TABLE B;







