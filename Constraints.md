# MySQL Constraints

In MySQL, **constraints** are rules applied to table columns to ensure accuracy, reliability, and integrity. Think of them as restrictions or conditions that the database enforces automatically.

## Common MySQL Constraints

1. **NOT NULL**  
   Ensures a column cannot have a `NULL` value.  
   Example: A `name` column with `NOT NULL` requires a value for every row.

2. **UNIQUE**  
   Ensures all values in a column are distinct.  
   Example: A `username` column with `UNIQUE` prevents duplicate usernames.

3. **PRIMARY KEY**  
   Combines `NOT NULL` and `UNIQUE` to uniquely identify each row in a table.  
   Example: A `user_id` column with `PRIMARY KEY` ensures each user has a unique ID.

4. **FOREIGN KEY**  
   Links a column in one table to a column in another table.  
   Example: An `Orders` table with a `user_id` column references the `user_id` in the `Users` table to ensure all orders are linked to valid users.

5. **DEFAULT**  
   Sets a default value for a column if no value is provided.  
   Example: A `status` column with `DEFAULT 'active'` automatically assigns `'active'` if no value is specified.

6. **CHECK**  
   Ensures values in a column meet a specific condition.  
   Example: A `price` column with `CHECK (price > 0)` ensures all prices are greater than zero.

7. **AUTO_INCREMENT**  
   Automatically generates a unique number for a column when a new row is added.  
   Example: An `id` column with `AUTO_INCREMENT` assigns IDs like 1, 2, 3, etc., to new rows.

---

These constraints help ensure the integrity and reliability of your data without requiring manual checks. 😊