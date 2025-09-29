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
