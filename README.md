# sql2
SQL Lesson 2 Drill

#bikeshare SQL drills 

#drill one: The ID's and durations for all trips of duration greater than 500, ordered by duration. every column for station id 84

SELECT\
    trip_id,\
	duration
FROM
    trips
WHERE
    duration >500 OR 
	duration = 500
ORDER BY duration DESC

#drill two: all columns for station id 84

SELECT  
    *  
FROM  
    stations  
WHERE  
    station_id = 84  

#drill three: min temperature for days with rain and zip code 94301

SELECT 
     MinTemperatureF
FROM 
    weather
WHERE 
    Events like 'rain' AND 
	ZIP = 94301
