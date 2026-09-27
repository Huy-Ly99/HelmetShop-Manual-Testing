# Test Data

> Do not store real customer personal information in this repository.

## Customer Data

| Field | Valid Data | Invalid Data |
|---|---|---|
| Name | Nguyen Van A | Empty / numeric-only |
| Phone | 0901234567 | Empty / invalid format |
| Address | 123 Nguyen Trai, HCMC | Empty |

## Product Data

| Case | Example |
|---|---|
| Normal price | 350000 |
| Minimum valid quantity | 1 |
| Quantity at stock boundary | Equal to stock |
| Quantity over stock | Stock + 1 |
| Empty product name | Invalid |
| Negative price | Invalid |

## Boundary Test Examples

- Quantity = 0
- Quantity = 1
- Quantity = stock - 1
- Quantity = stock
- Quantity = stock + 1
