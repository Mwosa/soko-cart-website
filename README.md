# 🛒 Soko Cart - E-Commerce Platform

A full-stack e-commerce application built with the MERN stack (MongoDB, Express.js, React.js, Node.js) featuring user authentication, product management, shopping cart functionality, and secure payment processing.

## ✨ Features

### 🛍️ User Features
- **User Authentication**: Secure login/register with JWT tokens
- **Product Browsing**: Browse products by categories with search functionality
- **Shopping Cart**: Add, remove, and update cart items with real-time persistence
- **Address Management**: Save and manage multiple delivery addresses
- **Order Management**: Place orders with COD or Stripe payment options

### 🏪 Seller Features
- **Seller Dashboard**: Dedicated seller authentication and dashboard
- **Product Management**: Add, edit, and manage product listings
- **Order Management**: View and manage incoming orders
- **Inventory Control**: Track product availability and stock

### 💳 Payment Integration
- **Cash on Delivery (COD)**: Traditional payment method
- **Stripe Integration**: Secure online payment processing

### 🛡️ Security Features
- **JWT Authentication**: Secure user sessions
- **Protected Routes**: Role-based access control
- **Input Validation**: Comprehensive form validation
- **Secure API**: Protected endpoints with middleware

## 🚀 Tech Stack

### Frontend
- **React.js** - User interface and state management
- **Vite** - Fast build tool and development server
- **Tailwind CSS** - Utility-first CSS framework
- **React Router** - Client-side routing
- **Axios** - HTTP client for API requests
- **React Hot Toast** - User notifications

### Backend
- **Node.js** - Server-side JavaScript runtime
- **Express.js** - Web application framework
- **MongoDB** - NoSQL database
- **Mongoose** - MongoDB object modeling
- **JWT** - JSON Web Token authentication
- **Stripe** - Payment processing
- **Cloudinary** - Image upload and management
- **bcryptjs** - Password hashing
- **CORS** - Cross-origin resource sharing

## 📋 Prerequisites

Before running this application, make sure you have the following installed:
- **Node.js** (v16 or higher)
- **npm** or **yarn**
- **MongoDB** (local or cloud instance)
- **Git**

## 🛠️ Installation & Setup

### 1. Clone the Repository
```bash
git clone https://github.com/Mwosa/soko-cart.git
cd soko-cart
```

### 2. Install Dependencies

**Install Backend Dependencies:**
```bash
cd server
npm install
```

**Install Frontend Dependencies:**
```bash
cd ../client
npm install
```

## 🚀 Running the Application

### Development Mode

**Start Backend Server:**
```bash
cd server
npm run dev
```
The backend will run on `http://localhost:4000`

**Start Frontend Development Server:**
```bash
cd client
npm run dev
```
The frontend will run on `http://localhost:5173`

### Production Build

**Build Frontend:**
```bash
cd client
npm run build
```

**Start Production Server:**
```bash
cd server
npm start
```

## 📁 Project Structure

```
soko-cart/
├── client/                 # Frontend React application
│   ├── src/
│   │   ├── components/     # Reusable UI components
│   │   ├── pages/         # Page components
│   │   ├── context/       # React context for state management
│   │   ├── assets/        # Static assets and images
│   │   └── main.jsx       # Application entry point
│   ├── public/            # Public assets
│   └── package.json       # Frontend dependencies
├── server/                # Backend Node.js application
│   ├── controllers/       # Route controllers
│   ├── models/           # MongoDB schemas
│   ├── routes/           # API routes
│   ├── middlewares/      # Custom middleware
│   ├── configs/          # Configuration files
│   └── server.js         # Server entry point
└── README.md             # Project documentation
```

## 🔧 API Endpoints

### Authentication
- `POST /api/user/register` - User registration
- `POST /api/user/login` - User login
- `GET /api/user/is-auth` - Check authentication status
- `GET /api/user/logout` - User logout

### Products
- `GET /api/product/list` - Get all products
- `POST /api/product/add` - Add new product (seller only)
- `GET /api/product/:id` - Get product details

### Cart
- `POST /api/cart/update` - Update cart items

### Orders
- `POST /api/order/cod` - Place COD order
- `POST /api/order/stripe` - Place Stripe order
- `GET /api/order/user` - Get user orders
- `GET /api/order/seller` - Get all orders (seller)

### Address
- `POST /api/address/add` - Add new address
- `GET /api/address/get` - Get user addresses

## 🔗 Live Demo

**Frontend:** [https://soko-cart.vercel.app](https://soko-cart.vercel.app)
**Backend API:** [https://soko-cart-backend.vercel.app/](https://soko-cart-backend.vercel.app/)

## 👥 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 🤝 Support

If you have any questions or need help with the project, please open an issue on GitHub or contact the development team.

---

**Built with ❤️ using the MERN stack** 
