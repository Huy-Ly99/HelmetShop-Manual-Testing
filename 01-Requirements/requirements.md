# HelmetShop – Requirements & Scope

## 1. Actors

### Customer
- Browse products
- View product details
- Add products to cart
- Update quantity
- Remove products
- Place an order

### Admin
- Log in
- Manage products
- View orders
- Update order status
- Manage completed/returned order records according to business rules

## 2. In Scope

1. Home page
2. Product listing
3. Product detail
4. Shopping cart
5. Checkout / order creation
6. Admin login
7. Product management
8. Order management
9. REST APIs
10. Database data validation
11. Responsive UI

## 3. Out of Scope

- Online payment gateway
- Customer account registration/login
- SMS/email notification
- Automated test framework

## 4. Business Rules to Verify

- Product quantity must not exceed available stock.
- Required customer information must be validated before order creation.
- An order cannot be created from an empty cart.
- Admin-only functions require valid authentication/authorization.
- Product and order data shown in the UI should be consistent with API/database data.
- Order status transitions must follow the implemented business flow.

> Update this document whenever the actual product requirements change.
