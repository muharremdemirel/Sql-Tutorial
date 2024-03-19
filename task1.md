Perform the following query scenarios using the dvdrental sample database.


1- Sort the data in the title and description columns in the movie table.

2- Sort the data in all columns in the movie table, with the movie length being greater than 60 AND less than 75.

3- Sort the data in all columns in the movie table as rental_rate 0.99 AND replacement_cost 12.99 OR 28.99.

4- What is the value in the last_name column of the customer whose value is 'Mary' in the first_name column in the customer table?

5- Sort the data in the movie table whose length is NOT greater than 50 and whose rental_rate value is NOT 2.99 or 4.99.


Solution:

1- select title, description from film;

2- select * from film where length > 60 and length < 75;

3- select * from film where rental_rate = 0.99 and (replacement_cost = 12.99 or replacement_cost = 28.99);

4- select last_name from customer where first_name = 'Mary';

5- select * from film where not (length > 50) and (rental_rate != 2.99 or rental_rate != 4.99);

