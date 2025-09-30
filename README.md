# Storefront

![GitHub last commit](https://img.shields.io/github/last-commit/mcna88/storefront)
![GitHub issues](https://img.shields.io/github/issues/mcna88/storefront)
![License](https://img.shields.io/github/license/mcna88/storefront)

**Storefront** is a modern backend application designed for managing online stores. It provides a clean and structured API for handling store operations efficiently.

## Features

- **Product Management:** Add, update, delete, and list products.
- **Collection & Inventory Management:** Organize products into categories and manage stock.
- **Order Management:** Create, update, and track customer orders.
- **User Authentication & Roles:** Secure login and role-based access control.
- **RESTful API:** Designed for integration with frontend applications or mobile apps.

## Installation

```bash
# Clone the repository
git clone https://github.com/mcna88/storefront.git
cd storefront

# Install dependencies using pipenv
pipenv install

# Activate the virtual environment
pipenv shell

# Apply migrations
python manage.py migrate

# Run the development server
python manage.py runserver
```

## API Documentation

Here are some of the main endpoints exposed by the API:

### Store Root
- `GET /store/` → API Root  
  Returns the available resources in the store, including:
  - `products` → `/store/products/`
  - `collections` → `/store/collections/`
  - `carts` → `/store/carts/`
  - `customers` → `/store/customers/`
  - `orders` → `/store/orders/`

### Authentication
- `POST /auth/users/` → Register a new user  
- `POST /auth/jwt/create/` → Login and obtain JWT token  

### Cart
- `POST /store/carts/` → Create a shopping cart  
- `GET /store/carts/{cart_id}/` → Retrieve cart details  
- `POST /store/carts/{cart_id}/items/` → Add item to cart  

### Orders
- `POST /store/orders/` → Create a new order  
- `GET /store/orders/` → List orders for the authenticated user  

### Admin
- `GET /admin/` → Django admin panel for managing products, users, and orders

