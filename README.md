# CURA - Healthcare Appointment Booking Platform

CURA is a full-stack web application that simplifies healthcare appointment booking. It connects patients with doctors through an intuitive platform featuring real-time appointment scheduling, secure payment processing, and comprehensive admin management tools.

## 🚀 Features

### For Patients (Users)
- Browse and search doctors by specialization
- View doctor profiles with availability
- Book, reschedule, and cancel appointments
- Secure online payment integration (Razorpay)
- Upload and manage medical documents
- View appointment history
- User authentication with JWT

### For Administrators
- Complete doctor management (Add/Edit/Remove)
- Appointment oversight and management
- Dashboard with analytics and statistics
- Revenue tracking and reports
- Image upload for doctor profiles
- Secure admin authentication

### Technical Highlights
- **Frontend**: React.js with Context API for state management
- **Backend**: Node.js with Express.js REST API
- **Database**: MongoDB with Mongoose ODM
- **Authentication**: JWT tokens with bcrypt encryption
- **Payment Gateway**: Razorpay integration
- **Cloud Storage**: Cloudinary for image management
- **File Upload**: Multer middleware
- **Security**: CORS, input validation, environment variables

## 📋 Prerequisites

Before running this project, make sure you have:

- Node.js (v14 or higher)
- npm or yarn
- MongoDB Atlas account (or local MongoDB)
- Cloudinary account
- Razorpay account (for payment integration)

## 🛠️ Installation & Setup

### 1. Clone the Repository
```bash
git clone https://github.com/10101AryAn101/CURA.git
cd CURA
```

### 2. Backend Setup

```bash
# Navigate to backend directory
cd backend

# Install dependencies
npm install

# Start the backend server
npm run server
# Server will run on http://localhost:4000
```

### 3. Admin Panel Setup

```bash
# Open new terminal and navigate to admin directory
cd admin

# Install dependencies
npm install

# Start the admin panel
npm run dev
# Admin panel will run on http://localhost:5174
```

### 4. Frontend Setup

```bash
# Open new terminal and navigate to frontend directory
cd frontend

# Install dependencies
npm install

# Start the frontend
npm run dev
# Frontend will run on http://localhost:5173
```

## 🚀 Running the Project

You need to run all three parts simultaneously:

1. **Backend Server** (Port 4000):
   ```bash
   cd backend
   npm run server
   ```

2. **Admin Panel** (Port 5174):
   ```bash
   cd admin
   npm run dev
   ```

3. **User Frontend** (Port 5173):
   ```bash
   cd frontend
   npm run dev
   ```

## 📁 Project Structure

```
CURA/
├── backend/              # Node.js + Express backend
│   ├── config/          # Database and Cloudinary config
│   ├── controllers/     # Business logic
│   ├── middleware/      # Auth and file upload middleware
│   ├── models/          # MongoDB schemas
│   ├── routes/          # API routes
│   └── server.js        # Entry point
│
├── admin/               # React admin dashboard
│   └── src/
│       ├── assets/      # Images and static files
│       ├── components/  # Reusable components
│       ├── context/     # Context API
│       └── pages/       # Admin pages
│
└── frontend/            # React user interface
    └── src/
        ├── assets/      # Images and static files
        ├── components/  # Reusable components
        ├── context/     # Context API
        └── pages/       # User pages
```

## 🔑 Default Admin Credentials

After setup, login to admin panel with:
- **Email**: admin@example.com (or as set in .env)
- **Password**: greatstack123 (or as set in .env)


## 📦 Dependencies

### Backend
- express - Web framework
- mongoose - MongoDB ODM
- jsonwebtoken - JWT authentication
- bcrypt - Password hashing
- multer - File upload
- cloudinary - Image storage
- razorpay - Payment gateway
- cors - Cross-origin resource sharing
- dotenv - Environment variables

### Frontend & Admin
- react - UI library
- react-router-dom - Routing
- axios - HTTP client
- react-toastify - Notifications



**Note**: Make sure to replace placeholder values in `.env` files with your actual credentials before running the project.
