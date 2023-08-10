## Cursor 

* a temporary work area
* stores the data retrieved from the database and manipulate this data
* hold more than one row, but can process only one row at a time.


### two types of cursors

Implicit cursor, and
explicit cursor

**Consistency** simply means that each user sees the consistent view of the data.

With **SAVEPOINT**, only part of transaction can be undone.

The **Rollback** statement is issued when the transaction ends. Following conditions are true for a Rollback statement:
The work done in a transition is undone as if it was never issued.
All locks acquired by transaction are released.

**Commit** statement
Other users can see the data changes made by the transaction.
The locks acquired by the transaction are released.
The work done by the transaction becomes permanent.

syntax error and runtime error

## cursor attributes used in PL/SQL?

%ISOPEN: it checks whether the cursor is open or not.

%ROWCOUNT: returns the number of rows affected by DML operations: INSERT,DELETE,UPDATE,SELECT.

%FOUND: it checks whether cursor has fetched any row. If yes - TRUE.

%NOTFOUND: it checks whether cursor has fetched any row. If no - TRUE.