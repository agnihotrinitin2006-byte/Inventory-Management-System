A REST API built with Node.js, Express.js, MongoDB and Mongoose to manage a product catalogue.

## Setup
1. `npm install`
2. Create a `.env` file:
   ```
   PORT=5000
   MONGO_URI=mongodb://127.0.0.1:27017/inventory_db
   ```
3. `node server.js`

## API Endpoints
| Method | URL | Purpose |
|---|---|---|
| POST | /api/products | Create product |
| GET | /api/products | List with filter, sort, pagination |
| GET | /api/products/:id | Get single product |
| PUT | /api/products/:id | Update product |
| PATCH | /api/products/:id/stock | Restock or sale |
| DELETE | /api/products/:id | Delete product |
| GET | /api/products/low-stock | Low-stock report |
| GET | /api/products/summary | Category-wise summary |

## Postman Screenshots

### Create Product (POST)
![Create](screenshots/create.png.png)

### Get Single Product (GET)
![Get Single](screenshots/get-single.png.png)

### Update Product (PUT)
![Update](screenshots/update(2).png.png)

### Stock Adjustment (PATCH)
![Stock](screenshots/stock-patch(2).png.png)

### Low-Stock Report (GET)
![Low Stock](screenshots/low-stock.png.png)

### Category Summary (GET)
![Summary](screenshots/summary.png.png)
=======