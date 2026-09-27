# API Testing

## Tools
- Postman

## API Areas

### Products
- GET products
- POST product
- PUT product
- DELETE product

### Cart
- POST cart
- GET cart
- POST cart item
- PUT cart item
- DELETE cart item

### Orders
- POST order
- Validate required customer fields
- Validate cart token
- Validate empty cart
- Validate stock

### Admin
- POST admin login
- Verify authentication token
- Verify protected endpoints

## API Checks

For each request verify:
- HTTP status code
- Response body
- Required fields
- Data types
- Error messages
- Boundary/negative cases
- Authentication/authorization
- Database impact
