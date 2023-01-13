# NewYork_Taxi_Trips
The code is a series of SQL queries that analyze data from the "bigquery-public-data.new_york_taxi_trips.tlc_green_trips_2018" table. The first query selects the pickup_datetime, fare_amount, and tip_amount columns from the table, and limits the results to 1000 rows.

The second query extracts the hour from the pickup_datetime column, and groups the results by hour. It then counts the number of trips that occurred in each hour, and orders the results by the number of trips in descending order.

The third query also extracts the hour from the pickup_datetime column, and groups the results by hour. It then calculates the average fare amount, average tip amount, and the percentage of the fare that the tip represents for each hour. The results are ordered by the average tip amount in descending order, to find the best hour for tips.

The fourth query uses the FORMAT_DATE function to extract the day of the week from the pickup_datetime column, and groups the results by the day of the week. It then counts the number of trips that occurred on each day of the week, and orders the results by the number of trips in descending order.

The fifth query also uses the FORMAT_DATE function to extract the day of the week from the pickup_datetime column, and groups the results by the day of the week. It then calculates the average fare amount, average tip amount, and the percentage of the fare that the tip represents for each day of the week. The results are ordered by the average tip amount in descending order, to find the best day of the week for tips.

The sixth query extracts the hour from the pickup_datetime column, and groups the results by hour. It then calculates the average fare amount, average tolls amount, and the percentage of the fare that the tolls represent for each hour. The results are ordered by the average tolls amount in descending order, to find the hour with the highest tolls.

The seventh query uses the FORMAT_DATE function to extract the day of the week from the pickup_datetime column, and groups the results by the day of the week. It then calculates the average fare amount, average tolls amount, and the percentage of the fare that the tolls represent for each day of the week. The results are ordered by the average tolls amount in descending order, to find the day of the week with the highest tolls.

The eighth query uses a subquery to calculate the average fare for each hour. It then uses the LAG function to find the previous fare for each hour, and orders the results by fare in descending order.

The ninth query uses a CTE (common table expression) to create a new table named daily_trips, which contains the date, the number of trips, and the total fare amount for each day. It then uses this table to calculate the average fare and number of trips for each month, and orders the results by the number of trips in descending order.
