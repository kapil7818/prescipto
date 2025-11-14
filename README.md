# Prescripto - Full-Stack Healthcare Appointment System

A comprehensive full-stack web application for managing healthcare appointments, built with modern technologies. This project includes a patient-facing frontend, an admin panel for management, and a robust backend API.

## 🚀 Features

### Patient Portal (Frontend)
- **User Registration & Authentication**: Secure login and signup with JWT tokens
- **Doctor Discovery**: Browse doctors by specialty with detailed profiles
- **Appointment Booking**: Easy scheduling with real-time availability
- **Payment Integration**: Support for Razorpay and Stripe payment gateways
- **Profile Management**: Update personal information and view appointment history
- **Responsive Design**: Mobile-friendly interface built with React and Tailwind CSS

### Admin Panel
- **Dashboard Analytics**: Overview of appointments, earnings, and user statistics
- **Doctor Management**: Add, edit, and manage doctor profiles
- **Appointment Oversight**: View and manage all appointments across the platform
- **User Management**: Monitor patient accounts and activities
- **Data Visualization**: Charts and metrics for business insights

### Backend API
- **RESTful API**: Well-structured endpoints for all operations
- **Authentication Middleware**: Role-based access control (Admin, Doctor, User)
- **Database Integration**: MongoDB with Mongoose ODM
- **File Upload**: Cloudinary integration for image storage
- **Payment Processing**: Secure payment handling with webhooks
- **Email Notifications**: Automated communication system

## 🛠️ Tech Stack

### Frontend
- **React 18** - Modern JavaScript library for building user interfaces
- **Vite** - Fast build tool and development server
- **Tailwind CSS** - Utility-first CSS framework
- **React Router** - Declarative routing for React
- **Axios** - HTTP client for API requests
- **React Toastify** - Notification system

### Backend
- **Node.js** - JavaScript runtime environment
- **Express.js** - Web application framework
- **MongoDB** - NoSQL database
- **Mongoose** - MongoDB object modeling
- **JWT** - JSON Web Tokens for authentication
- **bcrypt** - Password hashing
- **Multer** - File upload middleware
- **Cloudinary** - Cloud-based image management

### Payment Integration
- **Razorpay** - Indian payment gateway
- **Stripe** - Global payment processing

## 📁 Project Structure

```
prescripto-full-stack/
├── admin/                 # Admin panel (React + Vite)
│   ├── src/
│   │   ├── components/    # Reusable UI components
│   │   ├── context/       # React context for state management
│   │   ├── pages/         # Admin and doctor dashboard pages
│   │   └── assets/        # Static assets and icons
│   └── package.json
├── backend/               # Server-side API (Node.js + Express)
│   ├── controllers/       # Business logic handlers
│   ├── middleware/        # Authentication and validation
│   ├── models/           # MongoDB schemas
│   ├── routes/           # API endpoint definitions
│   ├── config/           # Database and cloud configurations
│   └── server.js         # Main server file
├── frontend/              # Patient portal (React + Vite)
│   ├── src/
│   │   ├── components/    # UI components
│   │   ├── pages/         # Application pages
│   │   ├── context/       # Global state management
│   │   └── assets/        # Images and icons
│   └── package.json
└── README.md
```

## 🔧 Installation & Setup

### Prerequisites
- Node.js (v16 or higher)
- MongoDB database
- Git

### Backend Setup
```bash
cd prescripto-full-stack/backend
npm install
# Create .env file with required environment variables
npm start
```

### Frontend Setup
```bash
cd prescripto-full-stack/frontend
npm install
npm run dev
```

### Admin Panel Setup
```bash
cd prescripto-full-stack/admin
npm install
npm run dev
```

## 🌐 Environment Variables

Create `.env` files in backend, frontend, and admin directories with the following variables:

### Backend (.env)
```
PORT=4000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
CLOUDINARY_NAME=your_cloudinary_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_SECRET_KEY=your_cloudinary_secret
RAZORPAY_KEY_ID=your_razorpay_key_id
RAZORPAY_KEY_SECRET=your_razorpay_key_secret
STRIPE_SECRET_KEY=your_stripe_secret_key
```

### Frontend (.env)
```
VITE_BACKEND_URL=http://localhost:4000
VITE_RAZORPAY_KEY_ID=your_razorpay_key_id
```

### Admin (.env)
```
VITE_BACKEND_URL=http://localhost:4000
```

## 🚀 Deployment

The application is configured for deployment on Vercel:

- **Frontend**: Deployed to `https://your-frontend-domain.vercel.app`
- **Admin Panel**: Deployed to `https://your-admin-domain.vercel.app`
- **Backend**: Deployed to `https://your-backend-domain.vercel.app`

Update the environment variables accordingly for production.

## 📱 Key Features Demonstration

### Patient Journey
1. **Registration/Login**: Secure user authentication
2. **Browse Doctors**: Filter by specialty and location
3. **Book Appointment**: Select date, time, and payment method
4. **Payment Processing**: Secure online payments
5. **Appointment Management**: View, reschedule, or cancel appointments

### Admin Capabilities
1. **Dashboard Overview**: Real-time statistics and metrics
2. **Doctor Management**: Add new doctors with credentials
3. **Appointment Monitoring**: Track all bookings and statuses
4. **User Administration**: Manage patient accounts

## 🔒 Security Features

- **Password Hashing**: bcrypt for secure password storage
- **JWT Authentication**: Token-based authentication system
- **Role-Based Access**: Different permissions for users, doctors, and admins
- **Input Validation**: Server-side validation for all inputs
- **CORS Configuration**: Proper cross-origin resource sharing setup

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the ISC License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

**Kapil** - [GitHub Profile](https://github.com/kapil7818)

## 🙏 Acknowledgments

- Built as a comprehensive full-stack project for portfolio demonstration
- Implements modern web development best practices
- Suitable for healthcare technology solutions

---

**Note**: This is a demonstration project. For production use, ensure proper security audits, testing, and compliance with healthcare regulations.
