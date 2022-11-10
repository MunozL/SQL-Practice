# SQL-Practice

SELECT *
FROM users
LIMIT 10;
 

SELECT *
FROM progress
LIMIT 10;
 

SELECT * 
FROM users 
WHERE email_domain Like '%.edu'
Limit 25;
 

SELECT city, Count(*) FROM users
WHERE city = 'New York';
 

SELECT mobile_app, Count(*)FROM users
WHERE mobile_app is NOT NUll
 

SELECT COUNT(sign_up_at),
  strftime('%H', sign_up_at) AS 'Sign up counts for each hour'
FROM users
GROUP BY  2
Limit 20;
 

SELECT u.user_id,
  u.email_domain,
  u.city,
  p.learn_cpp,
  p.learn_sql,
  p.learn_html,
  p.learn_javascript,
  p.learn_java
FROM users AS u
JOIN progress AS p 
  ON u.user_id = p.user_id
  WHERE u.city = 'New York' 
LIMIT 15;
 

SELECT u.email_domain,
  u.email_domain,
  u.city,
  p.learn_cpp,
  p.learn_sql,
  p.learn_html,
  p.learn_javascript,
  p.learn_java
FROM users AS u
JOIN progress AS p 
  ON u.user_id = p.user_id
  WHERE  u.city = 'Chicago'
LIMIT 15;
 

What did you like about this project?
I like that we were able to put in practice what we learned and challenge ourselves 
What did you struggle with in this project?
I struggled with  part 4. I don't think I got it 100% right but was able to get some of it
What would make your experience with this assessment better?
Having more knowledge about JOINS 
