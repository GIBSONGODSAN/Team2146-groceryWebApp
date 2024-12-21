# Grocery Store Shopping Cart App

This is a **MERN (MongoDB, Express, React, Node.js)** stack application that serves as a fully functional shopping cart system for a grocery store. It includes both backend and frontend implementations, along with various tools and features for deployment and development.

---

## Features

- User Authentication with **JWT** (JSON Web Tokens).
- Shopping cart with **add to cart**, **remove from cart**, and **update quantity** features.
- Product browsing with details.
- Payment integration using **PayPal**.
- Admin panel to manage products and orders.
- Responsive UI with **React-Bootstrap**.
- Data seeding and destruction functionality.

---

## Project Structure

- **Backend**: Handles API endpoints, database interaction, and business logic using **Express.js** and **MongoDB**.
- **Frontend**: Built using **React.js**, with state management handled by **Redux**.

---

## Installation and Setup

### 1. Clone the Repository
```bash
git clone https://github.com/your-repo/grocerystore.git
cd grocerystore
```

### 2. Install Dependencies
#### Install Backend Dependencies:
```bash
npm install
```

#### Install Frontend Dependencies:
```bash
cd frontend
npm install
cd ..
```

### 3. Environment Variables
Create a `.env` file in the root directory and configure the following variables:
```env
NODE_ENV=development
PORT=5000
MONGO_URI=<Your MongoDB connection string>
JWT_SECRET=<Your JWT secret>
PAYPAL_CLIENT_ID=<Your PayPal client ID>
```

---

## Scripts

### Backend
- **Start the server**:  
  ```bash
  npm run server
  ```
- **Import sample data**:  
  ```bash
  npm run data:import
  ```
- **Destroy sample data**:  
  ```bash
  npm run data:destroy
  ```

### Frontend
- **Start the client**:  
  ```bash
  npm run client
  ```

### Concurrently (Dev Mode)
- Start both frontend and backend together:  
  ```bash
  npm run dev
  ```

---

## Folder Structure

### Backend (`backend/`)
- **server.js**: Entry point for the backend.
- **routes/**: Contains Express route files for various functionalities.
- **models/**: Mongoose models for the application.
- **middleware/**: Middleware functions like authentication and error handling.
- **config/**: Database and other configurations.

### Frontend (`frontend/`)
- **src/**: React application source code.
- **components/**: Reusable React components.
- **screens/**: Page-level components.
- **redux/**: State management logic using Redux.

---

## Deployment

### Heroku Deployment
The app includes a `heroku-postbuild` script to build the frontend during deployment.

Steps:
1. Set up a Heroku project.
2. Push the code to the Heroku repository:
   ```bash
   git push heroku main
   ```

---

## Technologies Used

### Backend
- **Node.js**: JavaScript runtime environment.
- **Express.js**: Web framework for Node.js.
- **MongoDB**: NoSQL database for storing app data.
- **Mongoose**: MongoDB object modeling tool.
- **JWT**: Authentication tokens.
- **Multer**: File uploads.
- **Morgan**: HTTP request logger.

### Frontend
- **React.js**: Frontend framework.
- **React-Bootstrap**: Responsive UI components.
- **Redux**: State management.
- **Axios**: HTTP client.

---
