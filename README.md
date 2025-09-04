# 🩺 CareConnect – Role-Based Medical Appointment Booking Platform

CareConnect is a full-stack medical appointment platform that enables patients to seamlessly book appointments, doctors to manage their availability and approvals, and admins to onboard new doctors and control system-wide availability. It follows a **role-based architecture** (User, Doctor, Admin) and offers a production-grade UI prioritizing **mobile-first accessibility** and real-time workflows.


---
<p align="center">
  <img src="images/careconnect-logo.png" alt="CareConnect Logo" width="250"/>
</p>

---

## 🧠 Tech Stack

| Layer            | Technologies Used                   |
| ---------------- | ----------------------------------- |
| **Frontend**     | React.js, Tailwind CSS              |
| **Backend**      | Node.js, Express.js                 |
| **Database**     | MongoDB, Mongoose                   |
| **Auth**         | Clerk (OAuth + JWT), bcrypt         |
| **Payments**     | Stripe, Razorpay                    |
| **Media Upload** | Cloudinary                          |
| **Deployment**   | Vercel (Frontend), Render (Backend) |

---

## 🌟 Key Features

### 🔐 Clerk Authentication (OAuth + JWT)

- Seamless user sign-in via **Clerk**, including Google OAuth support  
- Backend protected with Clerk middleware for session-based access control  

### 🧑‍⚕️ Role-Based Dashboards

- **User Role:** Book appointments, browse doctors by specialty, make secure payments  
- **Doctor Role:** Approve/decline appointments, manage availability slots  
- **Admin Role:** Onboard new doctors, toggle availability, monitor appointments  

### 💳 Integrated Payments

- Secure online transactions via **Stripe** and **Razorpay**  
- Dynamic amount calculation, confirmation status, and real-time transaction feedback  

### ☁️ Media Storage with Cloudinary

- Doctor profile pictures uploaded securely and optimized using Cloudinary API  

### 🧠 Smart APIs & Filtering

- RESTful APIs built with **Express.js** supporting:
  - Specialty-based doctor search  
  - Role-based resource access  
  - Real-time status updates for appointments  

### 📱 Mobile-First UX

- Fully responsive layout ensuring optimal experience across all devices  

---

## 📦 Getting Started

### ✅ Prerequisites

- Node.js ≥ 18.x  
- MongoDB Atlas account  
- Clerk Project (Frontend + Backend API Keys)  
- Stripe + Razorpay Developer Keys  
- Cloudinary Account  

---

### 🔐 Default Admin Credentials

You can use the following admin credentials to test the **Admin Panel**:

- Email: admin@careconnect.com  
- Password: qwerty123  

---

## ⚙️ Installation Instructions

> 💡 Use **three separate terminals** to run `frontend`, `backend`, and `admin panel`.

### 📁 Clone the Repo

```bash
git clone https://github.com/pratiksindhiya/CareConnect.git
cd CareConnect
````

---

### 1️⃣ Start the Frontend (User App)

```bash
cd frontend
npm install
npm run dev
```

> 🌐 App runs on `http://localhost:5173`

---

### 2️⃣ Start the Backend (Open a new terminal)

```bash
cd CareConnect
cd backend
npm install
npm run dev
```

> 🚀 API runs on `http://localhost:5000`

---

### 3️⃣ Start the Admin Panel (Open another terminal)

```bash
cd CareConnect
cd admin
npm install
npm run dev
```

> 🧑‍⚕️ Admin Panel runs on `http://localhost:5174`

---

## ✅ Environment Variables

Create a `.env` file in both `backend` and `frontend/admin` as needed.

### Backend `.env` sample

```env
PORT=5000
MONGO_URI=your_mongodb_url
CLOUDINARY_CLOUD_NAME=your_cloudinary_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_secret
STRIPE_SECRET_KEY=your_stripe_key
RAZORPAY_KEY_ID=your_razorpay_id
RAZORPAY_SECRET=your_razorpay_secret
CLERK_SECRET_KEY=your_clerk_secret_key
```

---

## 🤝 Contributing

We welcome contributions from developers, designers, and product thinkers!

1. Fork the repo
2. Create a new branch (`git checkout -b feature/YourFeature`)
3. Commit your changes
4. Push and create a PR

---

## 👨‍💻 Author

**Pratik Sindhiya**
📧 Email: [pratiksindhiya3@gmail.com](mailto:pratiksindhiya3@gmail.com)
🔗 [GitHub](https://github.com/PRATIKSINDHIYA)

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

```

