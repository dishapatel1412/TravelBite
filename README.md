# TravelBite

##  Overview

TravelBite is a multi-vendor food ordering web application built with Laravel, PHP, MySQL, Blade, Bootstrap, and jQuery.

The platform allows customers to browse food items, add products to their cart, place orders, and make payments. Vendors can manage their food items and orders, while administrators can manage users, vendors, products, and other platform-level operations.

The project focuses on implementing a role-based, database-driven e-commerce workflow using Laravel.

---

##  Key Features

###  Customer

- User registration and authentication
- Browse available food items
- View food item details
- Add food items to cart
- Update cart quantities
- Remove items from cart
- Place orders
- Make online payments
- View order history
- View order details

###  Vendor

- Vendor authentication
- Manage food items
- Add food items
- Update food items
- Delete food items
- Manage incoming orders
- View order details
- Manage product availability

###  Administrator

- Manage users
- Manage vendors
- Manage food items
- Manage categories
- Manage orders
- Monitor platform activity
- Manage application data

---

##  Food & Product Management

TravelBite provides a food catalog where customers can browse available food items and view their details before placing an order.

Food items can be managed by vendors through their respective management interface.

### Food item functionality

- Add food items
- Edit food items
- Delete food items
- Upload food images
- Set food prices
- Associate food items with categories
- Manage food availability
- Display food items to customers

The food catalog is backed by a relational MySQL database and uses Laravel Eloquent relationships to connect related entities.

---

##  Cart Management

Customers can add food items to their cart before proceeding to checkout.

### Cart functionality

- Add food item to cart
- Update item quantity
- Remove item from cart
- View cart items
- Calculate order totals
- Proceed to checkout

The cart allows customers to review their selected items before placing an order.

---

##  Checkout & Payment Workflow

The ordering process follows a structured checkout workflow:

Browse Food Items
       ↓
View Food Details
       ↓
Add to Cart
       ↓
Review Cart
       ↓
Checkout
       ↓
Place Order
       ↓
Online Payment
       ↓
Payment Confirmation
       ↓
Order Created / Updated
       ↓
Order History

The payment workflow handles the interaction between the order and payment process before completing the customer's purchase.

---

##  Order Management

TravelBite provides order management for both customers and vendors.

### Customer

Customers can:

- Place orders
- View previous orders
- View order details
- Track the status of their orders

### Vendor

Vendors can:

- View incoming orders
- View order details
- Manage order status
- Process customer orders

This creates a complete order lifecycle from customer checkout to vendor order processing.

---

##  Role-Based Architecture

TravelBite is designed around multiple user roles.

                    TravelBite
                        │
        ┌───────────────┼───────────────┐
        ↓               ↓               ↓
    Customer          Vendor          Admin
        │               │               │
        ↓               ↓               ↓
     Browse          Products        Platform
     Cart            Orders          Management
     Orders
     Payments

Each role has access to functionality appropriate to its responsibilities.

Authorization and access control are used to prevent users from accessing functionality outside their role.

## 🗄️ Database Design

TravelBite uses **MySQL** as its relational database.

The application contains relationships between entities such as:

- Users
- Vendors
- Categories
- Food Items
- Cart
- Orders
- Order Items
- Payments

### Entity Relationship Diagram

### Application Flow

---

##  Laravel Concepts Used

TravelBite demonstrates several Laravel concepts, including:

- MVC architecture
- Routing
- Controllers
- Blade templates
- Eloquent ORM
- Eloquent relationships
- Migrations
- CRUD operations
- Authentication
- Authorization
- Middleware
- Form validation
- File and image handling
- Sessions
- Route model binding
- Database queries
- Query Builder / Eloquent
- Environment configuration
- Payment gateway integration
- Database relationships

---

##  Screenshots

### Customer Home Page

### Food Listing

### Food Details

### Shopping Cart

### Checkout

### Payment

### Customer Orders

### Vendor Dashboard

### Vendor Order Management

### Admin Dashboard

### Admin Management

---

##  Installation

### Prerequisites

Make sure the following are installed:

- PHP
- Composer
- MySQL
- Node.js & npm
- Laravel-compatible PHP extensions
- XAMPP / Laragon or another local PHP development environment

### 1. Clone the repository

git clone https://github.com/dishapatel1412/TravelBite.git
cd TravelBite

### 2. Install PHP dependencies

composer install

### 3. Install frontend dependencies

npm install

### 4. Create the environment file

cp .env.example .env

For Windows, create a copy of `.env.example` and rename it to `.env`.

### 5. Generate the application key

php artisan key:generate

### 6. Configure the database

Create a MySQL database and update the database configuration in `.env`:

DB_DATABASE=travelbite
DB_USERNAME=root
DB_PASSWORD=

### 7. Configure Razorpay

Add the required payment credentials to `.env`:

### 8. Run migrations

php artisan migrate

### 9. Build frontend assets

For development:

npm run dev

### 10. Start the Laravel development server

php artisan serve

The application will be available at:

http://127.0.0.1:8000

---

##  Future Improvements

Potential improvements for future versions include:

- Real-time order status updates
- Customer reviews and ratings
- Vendor analytics dashboard
- Advanced food search and filtering
- Coupon and discount management
- Delivery partner management
- Order notifications
- Email notifications
- REST API
- Automated test coverage expansion
- Caching and performance optimization
- Production deployment
- Mobile application

---

##  Tech Stack

### Backend

- PHP
- Laravel

### Frontend

- Blade
- HTML
- CSS
- Bootstrap
- JavaScript
- jQuery

### Database

- MySQL

### Payment

- Razorpay

### Development Tools

- Composer
- npm
- Vite
- Git
- GitHub
- XAMPP / Laragon

---

##  Author

**Disha Patel**

GitHub: [dishapatel1412](https://github.com/dishapatel1412)