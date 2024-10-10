# Inventory-Management-System

# Inventory Management API
This is a simple backend API for managing inventory items using Django Rest Framework, PostgreSQL, and Redis for caching.

## Setup
1. Install dependencies: `pip install -r requirements.txt`
2. Run migrations: `python manage.py migrate`
3. Start the server: `python manage.py runserver`
4. Set up Redis for caching.

## API Endpoints
- `POST /api/register/`: Register a new user.
- `POST /api/login/`: Obtain JWT token.
- `GET /api/items/`: List all items.
- `GET /api/items/{id}/`: Retrieve an item (cached using Redis).
- `POST /api/items/`: Create a new item.
- `PUT /api/items/{id}/`: Update an item.
- `DELETE /api/items/{id}/`: Delete an item.

## Running Tests
Run `python manage.py test` to execute unit tests.
