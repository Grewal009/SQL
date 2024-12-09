### SELECT statement

- The SELECT statement in SQL is used to fetch or retrieve data from a database. It allows users to access the data and retrieve specific data based on specific conditions.

```sql
SELECT column1,column2…. FROM table_name ;
```

#### Example

```sql
SELECT CustomerName, LastName FROM Customer;
```

#### Fetch All Table using SELECT Statement

```sql
SELECT * FROM Customer;
```

### SELECT Statement with WHERE Clause

```sql
SELECT CustomerName FROM Customer where Age = '21';
```

### SQL SELECT Statement with GROUP BY Clause

```sql
SELECT COUNT (item), Customer_id FROM Orders GROUP BY order_id;
```

### SELECT Statement with HAVING Clause

```sql
SELECT Department, sum(Salary) as Salary
FROM employee
GROUP BY department
HAVING SUM(Salary) >= 50000;
```

### SELECT Statement with ORDER BY clause in SQL

```sql
SELECT * FROM Customer ORDER BY Age DESC;
```

### Important Points

- It is used to access records from one or more database tables and views.
- The SELECT statement retrieves selected data based on specified conditions.
- The result of a SELECT statement is stored in a result set or result table.
- The SELECT statement can be used to access specific columns or all columns from a table.
- It can be combined with clauses like WHERE, GROUP BY, HAVING, and ORDER BY for more refined data retrieval.
- The SELECT statement is versatile and allows users to fetch data based on various criteria efficiently.
