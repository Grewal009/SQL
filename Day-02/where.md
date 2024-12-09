### WHERE Clause

The SQL WHERE clause is used to specify a condition while fetching or modifying data in a database.

```sql
SELECT column1,column2 FROM table_name WHERE column_name operator value;
```

```sql
SELECT * FROM Emp1 WHERE Age=24;
```

```sql
SELECT EmpID, Name, Country FROM Emp1 WHERE Age > 21;
```

### Where Clause with BETWEEN Operator

```sql
SELECT column1,column2 FROM table_name
WHERE column_name BETWEEN value1 AND value2;

SELECT * FROM Emp1 WHERE Age BETWEEN 22 AND 24;
```

### Where Clause with LIKE Operator

```sql
SELECT * FROM Emp1 WHERE Name LIKE 'S%';
```

- To fetch records of Employees where Name starts with the letter S.
- The ‘%'(wildcard) signifies the later characters here which can be of any length and value.

```sql
SELECT * FROM Emp1 WHERE Name LIKE '%M%';
```

### Where Clause with IN Operator

```sql
SELECT Name FROM Emp1 WHERE Age IN (21,23);
```

- It is used to fetch the filtered data same as fetched by ‘=’ operator just the difference is that here we can specify multiple values for which we can get the result set.

- Operators that Can be Used with WHERE Clause
  - `>` Greater Than
  - `>=` Greater than or Equal to
  - `<` Less Than
  - `<=` Less than or Equal to
  - `=` Equal to
  - `<>` Not equal to
  - `BETWEEN` In an inclusive Range
  - `LIKE` Search for a pattern
  - `IN` To specify multiple possible values for a column
