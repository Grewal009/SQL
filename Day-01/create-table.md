### Create Table

```sql
CREATE TABLE Customer(
    CustomerID INT PRIMARY KEY,
    CustomerName VARCHAR(50),
    LastName VARCHAR(50),
    Country VARCHAR(50),
    Age INT CHECK (Age >= 0 AND Age <= 99),
    Phone int(10)
);
```

### Insert data into table

```sql
INSERT INTO Customer (CustomerID, CustomerName, LastName, Country, Age, Phone)
VALUES (1, 'Shubham', 'Thakur', 'India',23,12121234),
       (2, 'Aman ', 'Chopra', 'Australia',21,12345612);
```

- if we specify all data in insert statemnt in the same order as columns in table:

  ```sql
  INSERT INTO Customer
      VALUES  (1, 'Shubham', 'Thakur', 'India',23,12121234),
              (2, 'Aman ', 'Chopra', 'Australia',21,12345612);

  ```

### Create Table From Another Table

```sql
CREATE TABLE student_name AS SELECT first_name,last_name from student;

```

### Command to check the structure of the table

```sql
DESC table_name;
```
