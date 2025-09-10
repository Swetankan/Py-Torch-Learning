
# 🎟️ Eventix – Event Ticketing & Management Platform

A modern full-stack **event management and ticketing platform**. With Eventix, users can **browse events, book tickets, and manage bookings**, while organizers can **host events, track sales, and verify tickets with QR codes**. Admins have full control over **users, categories, flagged events, and system analytics**.

🚀 **Live Demo (Vercel):** [https://eventix-demo.vercel.app](https://eventix-demo.vercel.app)

---

## ✨ Features

### 🎫 For Attendees
- Browse and search events by **category, location, and date**
- Secure ticket booking with **Stripe**
- **QR code tickets** for quick event entry
- Profile management & booking history
- **Google OAuth authentication**
- Flexible refund policy
- Contact organizers directly
- Report inappropriate events

### 🎤 For Organizers
- Create and manage events with images, venue map, and capacity
- Real-time booking analytics & revenue tracking
- **QR code ticket verification**
- Event cancellation with **automated refunds**
- Manage contact inquiries from attendees

### 🛠️ For Admins
- User & organizer management
- **Category management**
- Event reporting & moderation
- System-wide analytics & dashboards
- Contact message tracking
- Rate limiting & spam prevention

---

## 🛠 Tech Stack

**Frontend**
- React 19 + React Router
- TailwindCSS
- Axios
- React Hot Toast
- Date-fns

**Backend**
- Node.js + Express
- MongoDB + Mongoose
- JWT authentication + Google OAuth
- Stripe for payments
- Redis for caching & rate limiting
- Cloudinary for image uploads

---

## ⚡ Getting Started

### Prerequisites
- Node.js (v18+)
- MongoDB
- Redis
- Stripe Account
- Google OAuth & Maps API keys
- Cloudinary (for images)

### Installation

```bash
# Clone repo
git clone <repository-url>

# Navigate into the project directory
cd eventix

# Backend
cd backend
npm install

# Frontend
cd frontend
npm install
````

### Environment Setup

**Backend – `.env`**

```env
PORT=8000
CORS_ORIGIN=*
MONGODB_URI=mongodb://localhost:27017/Eventix
JWT_SECRET=your-secret
JWT_EXPIRES_IN=7d
NODE_ENV=development

GOOGLE_CLIENT_ID=your-google-client-id.apps.googleusercontent.com
STRIPE_SECRET_KEY=your-stripe-secret-key
GOOGLE_MAPS_API_KEY=your-google-maps-api-key

# Cloudinary
CLOUDINARY_CLOUD_NAME=your-cloudinary-cloud-name
CLOUDINARY_API_KEY=your-cloudinary-api-key
CLOUDINARY_API_SECRET=your-cloudinary-api-secret

# Redis
REDIS_HOST=localhost
REDIS_PORT=6379
```

**Frontend – `.env`**

```env
VITE_GOOGLE_CLIENT_ID=your-google-client-id.apps.googleusercontent.com
VITE_STRIPE_PUBLISHABLE_KEY=your-stripe-publishable-key
VITE_GOOGLE_MAPS_API_KEY=your-google-maps-api-key
```

### Run the Project

```bash
# In the backend directory
cd backend
npm run dev

# In a new terminal, in the frontend directory
cd frontend
npm run dev
```

🌍 App runs at: `http://localhost:5173`

-----

## 📚 API Endpoints

  - `POST /api/auth/register` – Register user
  - `POST /api/auth/login` – Login
  - `POST /api/events` – Create event (organizers)
  - `GET /api/events` – Fetch all events
  - `POST /api/bookings` – Book tickets
  - `POST /api/payments/create-payment-intent` – Stripe checkout
  - `POST /api/categories` – Add category (admin)
  - …and more\!

-----

## 📂 Project Structure

```
eventix/
├── backend/
│   ├── src/
│   │   ├── controllers/
│   │   ├── middleware/
│   │   ├── models/
│   │   ├── routes/
│   │   ├── utils/
│   │   └── server.js
│   └── package.json
└── frontend/
    ├── src/
    │   ├── components/
    │   ├── context/
    │   ├── pages/
    │   ├── services/
    │   ├── api/
    │   └── App.jsx
    └── package.json
```

-----

## 🌟 Contributing

1.  Fork this repo
2.  Create a feature branch (`git checkout -b feature/new-feature`)
3.  Commit your changes (`git commit -m "Added new feature"`)
4.  Push to the branch (`git push origin feature/new-feature`)
5.  Open a Pull Request

-----

## 📝 License

MIT License © 2025 Eventix

```

```
