# SQL injection cheat sheet

This note contains examples of useful syntax that you can use to perform a variety of tasks that often leverage your SQL injection attacks.


## `UNION SELECT` with sort

```sql
SELECT *
from user
where username='foo' and password='foo'
UNION select 1,2
ORDER by 1,2
```