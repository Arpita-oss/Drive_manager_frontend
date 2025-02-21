# Driver Management System (MERN Stack)

## 📌 Project Overview
The **Driver Management System** is a full-stack web application built using the **MERN stack** (MongoDB, Express.js, React.js, Node.js). It allows users to manage folders, subfolders, upload images, and organize data efficiently. The system supports authentication, nested folders, subfolders, image uploads, and a powerful search feature.

## ✨ Features
- **User Authentication** (Signup, Login, Logout)
- **Folder & Subfolder Management** (Create, Update, Delete, Organize Nested Folders & Subfolders)
- **Image Upload & Storage** (Upload images within folders and subfolders)
- **Search Functionality** (Find images by name)
- **Secure API with Authentication**

## 🛠️ Tech Stack
- **Frontend:** React.js, Tailwind CSS
- **Backend:** Node.js, Express.js
- **Database:** MongoDB
- **Authentication:** JSON Web Token (JWT)
- **State Management:** React Context API

## 📁 Folder Structure
```
📦 driver-management-system
├── 📂 client (React frontend)
│   ├── 📂 src
│   │   ├── 📂 components
│   │   ├── 📂 pages
│   │   ├── 📂 context
│   │   ├── App.js
│   │   ├── index.js
│   ├── package.json
│
├── 📂 server (Node.js backend)
│   ├── 📂 controllers
│   ├── 📂 models
│   ├── 📂 routes
│   ├── 📂 middleware
│   ├── server.js
│   ├── package.json
│
└── README.md
```

## 🚀 Installation & Setup

### 1️⃣ Clone the Repository
```sh
git clone https://github.com/your-username/driver-management-system.git
cd driver-management-system
```

### 2️⃣ Backend Setup
```sh
cd server
npm install  # Install dependencies
npm start    # Start the backend server
```

### 3️⃣ Frontend Setup
```sh
cd client
npm install  # Install dependencies
npm start    # Start the React frontend
```

### 4️⃣ Environment Variables
Create a `.env` file in the **server** folder and add:
```env
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key
```

## 🎯 API Endpoints
| Method | Endpoint                | Description                |
|--------|-------------------------|----------------------------|
| POST   | `/api/auth/signup`      | User Signup                |
| POST   | `/api/auth/login`       | User Login                 |
| GET    | `/api/folders`          | Fetch all folders          |
| POST   | `/api/folders/create`   | Create a new folder        |
| PUT    | `/api/folders/:id`      | Update a folder            |
| DELETE | `/api/folders/:id`      | Delete a folder            |
| GET    | `/api/subfolders`       | Fetch all subfolders       |
| POST   | `/api/subfolders/create`| Create a new subfolder     |
| PUT    | `/api/subfolders/:id`   | Update a subfolder         |
| DELETE | `/api/subfolders/:id`   | Delete a subfolder         |
| POST   | `/api/images/upload`    | Upload an image            |

## 🔒 Authentication
- Uses **JWT** tokens for secure authentication.
- Users must log in to manage folders, subfolders, and upload images.





