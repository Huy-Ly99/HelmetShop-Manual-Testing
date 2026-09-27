# Retest & Regression

## Retest Process

1. Developer changes/fixes the defect.
2. Tester verifies the original reproduction steps.
3. Record PASS or FAIL.
4. If FAIL, reopen the defect with new evidence.
5. If PASS, continue with regression testing.

## Regression Scope

When a change affects a feature, test related workflows.

Example: Cart change

```text
Product Detail
    ↓
Add to Cart
    ↓
Cart
    ↓
Update Quantity
    ↓
Delete Item
    ↓
Checkout
    ↓
Create Order
```

## Retest Record

| Bug ID | Build/Version | Result | Evidence | Final Status |
|---|---|---|---|---|
| BUG-001 |  |  |  |  |

## Regression Record

| Area | Test Cases | Passed | Failed | Blocked |
|---|---:|---:|---:|---:|
| Cart |  |  |  |  |
| Checkout |  |  |  |  |
| Orders |  |  |  |  |
| Admin |  |  |  |  |
