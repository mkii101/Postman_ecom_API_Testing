# Ecom Postman Collection

This repository contains a Postman collection for automating end-to-end API testing of an e-commerce application. The collection covers user authentication, product creation, order placement, order details retrieval, and product deletion.

## Collection Overview

The collection ([Ecom.postman-collection.json](007%20Ecom.postman-collection.json)) includes the following requests:

1. **Login**  
   Authenticates a user and stores the session token and user ID as collection variables.

2. **Create Product**  
   Adds a new product using form data, including product details and an image. Requires authentication.

3. **Create Order**  
   Places an order for the created product. Requires authentication.

4. **View Order Details**  
   Retrieves details of the placed order. Requires authentication.

5. **Delete Product**  
   Deletes the created product as a cleanup step. Requires authentication.

## How to Use

1. **Import the Collection**
   - Open Postman.
   - Click `Import` and select [007 Ecom.postman-collection.json](007%20Ecom.postman-collection.json).

2. **Set Up Variables**
   - The collection uses collection variables for `token`, `userId`, `productId`, `orderId`, and `productName`.
   - By default, `productName` is set to `Automation`. You can change this in the collection variables.

3. **Run the Collection**
   - Use the Collection Runner to execute all requests in sequence.
   - The scripts will automatically pass data (like token, productId, orderId) between requests.

4. **Image Upload**
   - The `Create Product` request requires a product image file. Update the `productImage` field in the request body to point to a valid image file on your system.

## Notes

- All requests use the base URL: `https://rahulshettyacademy.com/api/ecom/`
- Make sure your credentials in the `Login` request are valid.
- The collection includes test scripts to validate API responses and store variables for chaining requests.

## References

- [Postman Documentation](https://learning.postman.com/docs/getting-started/introduction/)
- [Rahul Shetty Academy APIs](https://rahulshettyacademy.com/)

---

**File:** [007 Ecom.postman-collection.json](007%20Ecom.postman-collection.json)