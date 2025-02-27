The `SELECT` statement is used to query data from a single table

For example to select all fields from commits table.

```sql
SELECT * FROM commits
```

Or Selecting just title and message

```sql
SELECT title message FROM commits
```

You can use Aggregation function in the select statement to perform function on all data until the current one

```sql
SELECT count(name) FROM commits
```

You can alias the column name only in this query by using `as` keyword for example

```sql
SELECT title as tt message FROM commits
SELECT name, commit_count, max(commit_count) AS max_count message FROM branches
```

You can select unique rows only using the `distinct` keyword for example,

```sql
SELECT DISTINCT title AS tt message FROM commits
```