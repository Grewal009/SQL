### DELETE Statement

The SQL DELETE statement is one of the most commonly used commands in SQL (Structured Query Language). It allows you to remove one or more rows from the table depending on the situation. Unlike the DROP statement, which removes the entire table, the DELETE statement removes data (rows) from the table retaining only the table structure, constraints, and schema

```sql
DELETE FROM Employees WHERE NAME = 'SAM';
```

### Deleting Multiple Records

```sql
DELETE FROM Employees
WHERE department = 'Development';
```

### Delete All of the Records

```sql
DELETE FROM EMPLOyees;
Or
DELETE * FROM EMPLOyees;
```

- All of the records in the table will be deleted, there are no records left to display. The table EMPLOyees will become empty.

### Rolling Back DELETE Operations

Since the DELETE statement is a DML operation, it can be rolled back when executed in a statement. If you accidentally delete records or need to repeat the process, you can use the ROLLBACK command.

```sql
START TRANSACTION;
DELETE FROM Employees WHERE department = 'Development';
-- If needed, you can rollback the deletion
ROLLBACK;
```

- Use Transactions: Wrap DELETE statements in transactions to provide an option to roll back changes if necessary.
- Always Use a WHERE Clause: Avoid deleting all rows by accident. Always filter records using a WHERE clause to specify which rows to delete.
