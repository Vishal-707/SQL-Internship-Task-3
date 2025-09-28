# SQL-Internship-Task-3
# SQL-Internship-Task-3
The objective of this task was to practice writing basic SELECT queries to extract data from one or more tables.
# Used Tools 
<b> MySQL Workbench <b> <br>
I used this tool to connect to a local database server, create the E-commerce database, and run the provided SQL script.
### *Queries and Concepts*
The provided SQL script was used to create and populate the following tables: Customers, Products, Orders, and Payments. I then executed a series of SELECT queries to answer specific questions, demonstrating my understanding of core SQL concepts. <br>
## Concepts 

| Command      | Definition                                                                |
| ------------ | ------------------------------------------------------------------------- |
| `SELECT`     | Retrieves data from one or more tables.                                   |
| `FROM`       | Specifies the table to retrieve data from.                                |
| `WHERE`      | Filters records based on specified condition(s).                          |
| `AND` / `OR` | Combines multiple conditions in the `WHERE` clause.                       |
| `ORDER BY`   | Sorts the result set in ascending (`ASC`) or descending (`DESC`) order.   |
| `LIMIT`      | Limits the number of rows returned.                                       |
| `BETWEEN`    | Filters results within a specified range.                                 |
| `LIKE`       | Searches for a specified pattern in a column (not used here, but useful). |

---
## SELECT 
The SELECT command is used to retrieve specific columns | All columns using * from one or more tables. 

* Syntax - Show  All Column  <br>
  ```sql
   SELECT * FROM Table_Name;
  ``` 
* Syntax - Show Specific Columns <br>
  ```sql
  SELECT column1,column2,.... columnN FROM Tablename;
  ```
* Syntax of See data filtered by a condition. <br>
  ```sql
  SELECT * FROM TableName WHERE Column1 = 'Value';
  ```
##  WHERE
Filters records based on one or more specified conditions. Only rows where the condition is true are included in the result set.
* Syntax <br>
```sql
    SELECT * FROM Table_Name WHERE Condition ;
```
# AND 
Logical operators used within the WHERE clause to combine multiple conditions. AND requires both conditions to be true, while OR requires at least one condition to be true.

* Syntax of AND <br>

  ```sql
    SELECT * FROM Table_Name WHERE condition1 AND condition2;
  ```
* Syntax of OR <br>
  ```sql
    SELECT * FROM Table_Name WHERE condition1 OR condition2;
   ```
* Syntax of And OR 
  ```sql
    SELECT * FROM Table_Name WHERE condition1 AND condition2 WHERE condition1 OR condition2;
  ```
# ORDER BY 
Sorts the result set based on the values in one or more columns. The sorting can be in ascending (ASC) or descending (DESC) order.
The Sorting result in Asceding order by Use ASC keyword . Descending order by useing by DESC keyword. By default order by sorts in ascending order.
 *  Syntax <br>
   ```sql
  SELECT * FROM Table_Name ORDER BY column1 [ASC/DESC] ;
   ```
* Syntax with condition  <br>
  ```sql
  SELECT * FROM Table_Name WHERE Condition ORDER BY Column1 [ASC/DESC] ;
  ```
# LIMIT
Restricts the number of rows returned by the query. Essential for efficiency and pagination.

  * Syntax of Limit <br>
  ```sql
  SELECT * FROM Table_Name WHERE Condition  LIMIT Number_of_row ;
  ```

# BETWEEN
An operator used in the WHERE clause to filter results within an inclusive range of values including the start and end values.
* Syntax <br>

   ```sql
    SELECT * FROM Table_Name WHERE column_name BETWEEN value1 AND value2 ;
   ```
# LIKE
An operator used in the WHERE clause to search for a specified pattern in a column. It uses wildcard characters % for any sequence of characters, _ for any single character .
*  LIKE with wildcard % Matches any sequence of characters.

1. First Value - a%
2. Last Value - %a
3. To check middle string - %a% <br>

* LIKE with wildcard _ <br>
i. Matches exactly one Character. <br>

* Syntax
  ```sql
  SELECT column1, column2 FROM Table_Name WHERE column_name LIKE 'pattern';
  ```



