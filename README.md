Book Store - Node Express
Book Store is a web application built with Node.js and Express that allows users to browse, search, and purchase books. The app provides a robust backend to manage books, user authentication, and order processing.

Table of Contents
Introduction
Features
Installation
Usage
API Endpoints
Project Structure
Introduction
The Book Store application is designed to provide an easy and convenient platform for users to buy books online. It includes functionalities for browsing books by category, searching for specific books, user authentication, and managing orders.

Features
Browse books by category
Search for specific books
View detailed information about books
User authentication and profile management
Manage shopping cart and place orders
Installation
Clone the repository:
git clone https://github.com/Chukwuskindall/book-store-rest-api.git
cd Book-Store-Node-Express
Install dependencies:
npm install
Set up environment variables:
Create a .env file in the root directory and add your environment variables:

DB_HOST=your_database_host
DB_USER=your_database_user
DB_PASS=your_database_password
JWT_SECRET=your_jwt_secret
Run the application:
npm start
The server will start on http://localhost:3000.

Usage
Open your web browser and navigate to http://localhost:3000.
Sign up or log in to your account.
Browse through the list of books.
Search for books using the search bar.
View book details by clicking on a book.
Add books to your shopping cart.
Proceed to checkout and place your order.
API Endpoints
Books
GET /api/books: Retrieve all books
GET /api/books/:id: Retrieve a specific book
POST /api/books: Add a new book (admin only)
PUT /api/books/:id: Update a book (admin only)
DELETE /api/books/:id: Delete a book (admin only)
Users
POST /api/users/signup: Sign up a new user
POST /api/users/login: Log in a user
GET /api/users/profile: Retrieve user profile (authenticated users only)
PUT /api/users/profile: Update user profile (authenticated users only)
Orders
GET /api/orders: Retrieve all orders (admin only)
GET /api/orders/:id: Retrieve a specific order (authenticated users only)
POST /api/orders: Place a new order (authenticated users only)
Project Structure
Book-Store-Node-Express/
│
├── controllers/             # Controller files for handling requests
├── models/                  # Database models
├── routes/                  # Route definitions
├── middlewares/             # Middleware functions
├── config/                  # Configuration files
├── utils/                   # Utility functions
├── .env                     # Environment variables
├── app.js                   # Main application file
├── package.json             # Project dependencies
└── README.md                # Project README file
