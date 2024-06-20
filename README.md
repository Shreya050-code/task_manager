# Task Management Application (MERN Stack)

This is a Task Management Application built using the MERN stack (MongoDB, Express, React, Node.js). It allows users to manage tasks with CRUD operations (Create, Read, Update, Delete).

## Prerequisites

Before you begin, ensure you have the following installed on your system:

- Node.js - Download and install [Node.js](https://nodejs.org/en/download/)

## Getting Started

Follow these steps to set up and run the project locally:

### 1. Clone the Repository

```bash
git clone https://github.com/Shreya050-code/task_manager
cd task_manager-master
```

### 2. Install Dependencies

#### Backend

```bash
cd task-backend
npm install
```

#### Frontend

```bash
cd task-frontend
npm install
```

### 3. Set Environment Variables Backend

Create a `.env` file in the `task-backend` directory and add the following:

```plaintext
MONGO_URL=mongodb+srv://Shreya050:Shreya0501@cluster0.4kjv9so.mongodb.net/?retryWrites=true&w=majority&appName=Cluster0
SECRET_KEY="Shreya"
```

Replace `MONGO_URL` with your MongoDB connection string and `SECRET_KEY` with a random string for JWT token encryption.


### 4. Start the Backend Server

```bash
cd task-backend
nodemon start
```

The backend server will start running at `http://localhost:8000`.

### 5. Set Environment Variables Backend

Create a `.env` file in the `task-frontend` directory and add the following:

```plaintext
VITE_API_URL="http://localhost:8000/api"
```

Replace `VITE_API_URL` with the local backend server running at port 8000 as shown above or you can replace it with the url in which your backend is hosted in production.

### 6. Start the Frontend Development Server

Open a new terminal and navigate to the `task-frontend` directory:

```bash
cd task-frontend
npm run dev
```

The frontend development server will start running at `http://localhost:5173`.

### 7. Access the Application

Open your web browser and visit `http://localhost:5173` to access the Task Management Application.

## Additional Notes
- The application uses certain confidential information in your `.env` file that is kept secure and confidential.
