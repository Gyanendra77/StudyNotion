# StudyNotion – MERN EdTech Platform

A full-stack learning platform where instructors can create courses and learners can enroll, track progress, and earn skills. Built with the MERN stack and designed for scalability, clean code, and developer friendliness.

> **Tech:** MongoDB, Express.js, React, Node.js (MERN) • JWT Auth • Cloud Storage • Email/OTP • (Optional) Payments

---

## ✨ Features

- **Auth & Security**
  - Signup/Login with **JWT** and hashed passwords
  - **Email OTP** verification & password reset links
  - Role-based access (**Student / Instructor / Admin**)
- **Course Management**
  - Create, edit, publish/unpublish courses
  - Sections & lectures (video/text), rich descriptions, prerequisites, tags
  - Course thumbnails & media uploads (Cloudinary/S3)
- **Learning Experience**
  - Secure **video player**, progress tracking, notes
  - Ratings & reviews, course search & filters
  - Wishlists, “Continue Learning”, and completion certificates (optional)
- **Dashboards**
  - **Instructor:** revenue, enrollments, course analytics
  - **Student:** enrolled courses, progress, wishlist
- **(Optional) Payments**
  - Razorpay/Stripe integration for paid courses
- **Developer Experience**
  - Environment-based config
  - API-first design, modular controllers/services
  - Ready CI/CD & Docker (optional)

---

## 🗂️ Monorepo Structure


---

## 🚀 Quick Start

### 1) Clone & Install

```bash
git clone https://github.com/<your-username>/StudyNotion.git
cd StudyNotion

# Install server deps
cd server && npm install

# Install client deps
cd ../client && npm install

2) Environment Variables
Create server/.env:

# Server
PORT=4000
MONGODB_URI=mongodb://localhost:27017/studynotion
JWT_SECRET=your_super_secret_jwt_key
JWT_EXPIRES_IN=7d

# OTP / Email (Nodemailer)
MAIL_HOST=smtp.gmail.com
MAIL_PORT=587
MAIL_USER=your_email@gmail.com
MAIL_PASS=your_app_password

# Cloud Storage (Cloudinary example)
CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_key
CLOUDINARY_API_SECRET=your_secret

# (Optional) Payments
RAZORPAY_KEY_ID=your_key_id
RAZORPAY_KEY_SECRET=your_key_secret
STRIPE_SECRET_KEY=your_stripe_secret
FRONTEND_URL=http://localhost:5173




