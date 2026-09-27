# Database Testing

## Tool
DBeaver

## Main Tables
- products
- carts
- cart_items
- orders
- order_items

## Validation Examples

### Verify latest orders
```sql
SELECT *
FROM orders
ORDER BY created_at DESC;
```

### Verify order items
```sql
SELECT *
FROM order_items
WHERE order_id = <ORDER_ID>;
```

### Verify product stock
```sql
SELECT id, name, stock
FROM products
ORDER BY id;
```

## What to Validate

- UI order data matches database data.
- Order total is correct.
- Order items reference the correct products.
- Quantity is correct.
- Product stock changes according to the implemented business rule.
- Status changes are persisted correctly.
