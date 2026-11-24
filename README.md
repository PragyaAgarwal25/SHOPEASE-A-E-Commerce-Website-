# ShopEase – E-Commerce Website

ShopEase is a web-based e-commerce application developed to provide customers with a simple and convenient online shopping experience. It allows customers to browse products, manage their shopping cart, place orders, and track order status.

The application also provides an Admin Panel to manage products, categories, customers, orders, and stock information.

## Features

### Customer Features
- Customer registration and login
- Secure password hashing
- Browse available products
- Add products to shopping cart
- Place customer orders
- View order history
- Track order status

### Admin Features
- Admin authentication
- Admin dashboard with statistics
- Add, update, and delete products
- Manage customer orders
- Update order status
- Monitor product stock

## Technologies Used

| Technology | Purpose |
|---|---|
| HTML | Webpage structure |
| CSS | Website styling |
| JavaScript | Frontend functionality |
| Node.js | Backend runtime |
| Express.js | Backend framework |
| MySQL | Database |
| MySQL Workbench | Database management |
| bcryptjs | Password hashing |
| JWT | Authentication |
| CORS | Cross-origin requests |

## Project Structure

```text
ShopEase/
│
├── backend/
│   ├── config/
│   │   └── db.js
│   ├── middleware/
│   │   └── auth.js
│   └── server.js
│
├── frontend/
│   ├── css/
│   │   └── style.css
│   ├── js/
│   │   └── app.js
│   └── index.html
│
├── database/
│   └── SQL files
│
├── .env.example
├── .gitignore
├── package.json
├── package-lock.json
└── README.md
```

## Prerequisites

Before running the project, install:

- Node.js
- npm
- MySQL Server
- MySQL Workbench (recommended)
- Visual Studio Code

## Installation and Setup

### 1. Clone the Repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

### 2. Open the Project Folder

```bash
cd ShopEase
```

### 3. Install Dependencies

```bash
npm install
```

### 4. Configure Environment Variables

Create a `.env` file in the project root directory using `.env.example`.

Example configuration:

```env
PORT=5000
DB_HOST=localhost
DB_USER=root
DB_PASSWORD=your_mysql_password
DB_NAME=shopease
JWT_SECRET=your_secret_key
```

Replace the example values with your own MySQL credentials and secret key.

### 5. Setup Database

1. Open MySQL Workbench.
2. Create a database named `shopease`, if it is not created by the SQL script.
3. Open the SQL file available in the `database` folder.
4. Execute the SQL script to create the required tables, views, triggers, and stored procedures.

### 6. Run the Project

```bash
npm run dev
```

The backend server will run at:

```text
http://localhost:5000
```

Open the application in your browser using the configured frontend route.

## Database Design

The project uses a MySQL relational database named `shopease`.

Main database tables:

| Table | Description |
|---|---|
| Users | Stores customer and admin information |
| Categories | Stores product categories |
| Products | Stores product details and stock |
| Orders | Stores customer order information |
| Order_Items | Stores individual items in orders |
| Stock_Audit | Records stock changes |

### Database Concepts Implemented

- Primary Keys and Foreign Keys
- SQL Joins
- Subqueries
- Views
- Stored Procedures
- Triggers
- Aggregate Functions
- Relational Database Design

## Security

- Passwords are hashed using bcryptjs.
- JWT-based authentication is implemented.
- Protected routes are used for authenticated users.
- Admin-only access is provided for administrative operations.
- Sensitive configuration values are stored in environment variables.

## Future Enhancements

- Online payment gateway integration
- Product reviews and ratings
- Wishlist functionality
- Email notifications
- Advanced search and filtering
- Delivery tracking

## Project Purpose

This project was developed as an academic project to demonstrate practical knowledge of web development, backend programming, database management, and SQL concepts.

## Authors

**Project:** ShopEase – E-Commerce Website

**Developed using:** HTML, CSS, JavaScript, Node.js, Express.js and MySQL.
