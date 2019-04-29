# Joining-Data-in-SQL-in-DataCamp-Course
# Chapter 1

SELECT * 
FROM cities
-- 1. Inner join to countries
INNER JOIN countries
-- 2. Match on the country codes
ON cities.country_code = countries.code;
      
    
-- 1. Select name fields (with alias) and region 
SELECT cities.name AS city, countries.name AS country, region
FROM cities
INNER JOIN countries
ON cities.country_code = countries.code;

-- 3. Select fields with aliases
SELECT c.code AS country_code, name, year, inflation_rate
FROM countries AS c
-- 1. Join to economies (alias e)
INNER JOIN economies AS e
-- 2. Match on code
ON c.code = e.code;

SELECT c.code, c.name, c.region, p.fertility_rate, p.year
FROM countries AS c
INNER JOIN populations AS p
ON c.code = p.country_code


-- 6. Select fields
SELECT c.code, c.name, c.region, p.year, p.fertility_rate
-- 1. From countries (alias as c)
FROM countries AS c
-- 2. Join to populations (as p)
INNER JOIN populations AS p
-- 3. Match on country code
ON c.code = p.country_code
-- 4. Join to economies (as e)
INNER JOIN economies as e
-- 5. Match on country code
ON c.code = e.code  ;


-- 6. Select fields
SELECT c.code, name, region, e.year, fertility_rate, unemployment_rate
-- 1. From countries (alias as c)
FROM countries AS c
-- 2. Join to populations (as p)
INNER JOIN populations AS p
-- 3. Match on country code
ON c.code = p.country_code
-- 4. Join to economies (as e)
INNER JOIN economies AS e
-- 5. Match on country code and year
ON c.code = e.code
AND e.year = p.year;
