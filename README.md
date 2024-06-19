# SQL-SELECT-Statement    
-- Select all data from the users table
SELECT * FROM users;

-- Count the number of users in each country
SELECT country, COUNT(*) AS number_of_users
FROM users
GROUP BY country
ORDER BY number_of_users DESC;

-- Find the average age of users
SELECT AVG(age) AS average_age
FROM users;

-- List the top 5 most used social media platforms
SELECT platform, COUNT(*) AS usage_count
FROM user_activity
GROUP BY platform
ORDER BY usage_count DESC
LIMIT 5;
