# Dropshipping Platform

A comprehensive dropshipping platform with Django backend and React frontend.

## Project Structure

- `dropshipping-platform/` - Django backend
- `front/my-app/` - React frontend

## Backend Setup

1. Install dependencies:
   ```
   cd dropshipping-platform
   pip install -r requirements.txt
   ```

2. Run migrations:
   ```
   python manage.py migrate
   ```

3. Create a superuser:
   ```
   python manage.py createsuperuser
   ```

4. Run the server:
   ```
   python manage.py runserver
   ```

## Frontend Setup

1. Install dependencies:
   ```
   cd front/my-app
   npm install
   ```

2. Run the development server:
   ```
   npm start
   ```

## API Endpoints

The backend provides the following API endpoints:

- `/api/users/` - User management
- `/api/profiles/` - User profiles
- `/api/suppliers/` - Supplier management
- `/api/product-types/` - Product types
- `/api/products/` - Product management
- `/api/sellers/` - Seller management
- `/api/seller-orders/` - Order management
- `/api/deliverers/` - Deliverer management
- `/api/deliveries/` - Delivery management
- `/api/auth/login/` - User login
- `/api/auth/logout/` - User logout

## Authentication

The platform uses session-based authentication. To authenticate:

1. Send a POST request to `/api/auth/login/` with username and password
2. The server will set a session cookie
3. Include the cookie in subsequent requests using `credentials: 'include'`

## CORS Configuration

The backend is configured to allow requests from the React frontend running on `http://localhost:3000`.
