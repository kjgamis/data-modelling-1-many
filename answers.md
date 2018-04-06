## Exercises
The data in this part of the assignment uses the ```authors```, ```articles```, ```countries```, ```provinces```, ```cities```, ```residences```, and ```persons``` tables from earlier in the assignment.

Write SQL queries (in as many steps as necessary) to solve each of the following:

1. Find the author with the name 'Kara Melton' and then select all the articles she has written.
  ```
  SELECT * FROM authors WHERE name = 'Kara Melton';
  ```
2. Find Ontario in the provinces table and then find all the cities in that province.
  ```
  SELECT * FROM provinces WHERE name = 'Ontario';
  SELECT * FROM cities WHERE province_id = 14;
  ```
3. Who wrote the article called 'Coding Bootcamps and Emotional Labor'?
  ```
  SELECT author_id FROM articles WHERE title = 'Coding Bootcamps and Emotional Labor'; => 4
  SELECT name FROM authors WHERE id = 4; => Tilde Ann Thurium
  ```
4. Write a series of SQL queries to find out how many provinces are in Canada.
  ```
  SELECT COUNT (id) FROM provinces; => 14
  ```
5. How many people live at 4740 McDermott Street?
  ```
  SELECT * FROM residences WHERE address = '4740 McDermott Street';
  SELECT * FROM persons WHERE residence_id = 9;
  ```
6. What city is 4740 McDermott Street in?
  ```
  SELECT * FROM residences WHERE address = '4740 McDermott Street'
  ```
7. What province is 4740 McDermott Street in?
  ```

  ```
8. What country is 4740 McDermott Street in?
  ```

  ```
9. Find the person named 'Destini Davis' and then use a series of SQL queries to find what country they live in.
  ```

  ```
10. How many articles has Aditya Mukerjee written?
  ```

  ```
