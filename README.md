# Sql-weather-Data
--1. Find all records where the weather was exactly clear.
SELECT *
FROM   Weather_Data
WHERE  weather = 'Clear';

--2.Find the number of times the wind speed was exactly 4 km/hr.
SELECT *
FROM   Weather_Data
WHERE  wind_speed_km_per_h = 4;

-- 3.What is the mean visibility of the dataset?
SELECT AVG(Visibility_km) AS visibility_mean
FROM    Weather_Data;


--4.Find the number of records where the wind speed is greater than 24 km/hr and visibility is equal to 25 km.
SELECT wind_speed_km_per_h,Visibility_km
FROM   Weather_Data
WHERE  Visibility_km = 25 AND wind_speed_km_per_h >24;
