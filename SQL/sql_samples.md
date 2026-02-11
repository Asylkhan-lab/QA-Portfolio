# SQL Samples (Basic)

```sql
-- 1) Find users with gmail addresses
SELECT id, email
FROM users
WHERE email LIKE '%@gmail.com';

-- 2) Orders with customer names (JOIN)
SELECT o.id, o.created_at, c.name
FROM orders o
JOIN customers c ON c.id = o.customer_id
WHERE o.created_at >= '2026-01-01';

-- 3) Count orders per customer
SELECT c.name, COUNT(*) AS orders_count
FROM orders o
JOIN customers c ON c.id = o.customer_id
GROUP BY c.name
ORDER BY orders_count DESC;
```
