# -data-engineering-zoomcamp-homework1

1 - Knowing docker tags

B) --iidfile string

2 - Understanding docker first run
C) 3

3 - Count records
B) 20530

SELECT COUNT(1)
FROM green_taxi_data 
WHERE
CAST(tpep_pickup_datetime AS DATE) = '2019-01-15' 
AND 
CAST(tpep_dropoff_datetime AS DATE) = '2019-01-15' 

4. Largest trip for each day

C) 2019-01-15
SELECT *
FROM green_taxi_data ORDER BY trip_distance DESC LIMIT 10

Question 5. The number of passengers

SELECT COUNT(1) FROM green_taxi_data WHERE passenger_count = 2 AND CAST(lpep_pickup_datetime AS DATE) = '2019-01-01' 
SELECT COUNT(1) FROM green_taxi_data WHERE passenger_count = 3 AND CAST(lpep_pickup_datetime AS DATE) = '2019-01-01' 

C) 2: 1282 ; 3: 254
