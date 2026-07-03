# 🎙️ Wish AI — Embeddable AI Voice Assistant

<div align="center">

### Build a custom AI voice assistant for your business and embed it into any website with a single script.

![React](https://img.shields.io/badge/React-19-61DAFB?style=for-the-badge\&logo=react)
![Node.js](https://img.shields.io/badge/Node.js-Express-339933?style=for-the-badge\&logo=node.js)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge\&logo=mongodb)
![Google Gemini](https://img.shields.io/badge/Google-Gemini-4285F4?style=for-the-badge\&logo=google)
![Firebase](https://img.shields.io/badge/Firebase-Authentication-FFCA28?style=for-the-badge\&logo=firebase)
![Tailwind CSS](https://img.shields.io/badge/Tailwind-CSS-06B6D4?style=for-the-badge\&logo=tailwindcss)

### 🚀 Live Demo

**🔗 https://wishai.onrender.com/**

</div>

---

## 📌 Quick Links

* 🌐 **Live Demo:** https://wishai.onrender.com/
* 💻 **Repository:** https://github.com/ArcSaber21/AIVoiceAgent

---

# 📖 Overview

**Wish AI** is a full-stack SaaS platform that lets businesses create their own AI-powered voice assistant without writing any code.

Users can sign in using Google, describe their business, choose an assistant personality, customize the widget appearance, and instantly receive an embeddable AI assistant that can answer visitor questions and navigate users around the website using voice commands.

The project is built as a **monorepo** consisting of:

```text
client/   → React Dashboard
server/   → Node.js + Express Backend
```

---

# ✨ Features

## 🤖 AI Assistant Builder

* Custom assistant name
* Business information configuration
* Business category & description
* Multiple assistant personalities

  * Friendly
  * Professional
  * Sales
* Multiple widget themes

  * Light
  * Dark
  * Glass
  * Neon

---

## 🔐 Authentication

* Google Sign-In
* Firebase Authentication
* JWT Session Cookies
* Protected Dashboard Routes

---

## 🎤 AI Powered Conversations

* Powered by Google Gemini
* Bring Your Own Gemini API Key
* Automatic API Key Validation
* Live API Status

```text
✅ Active
❌ Invalid
⚠️ Quota Exceeded
```

---

## 🌐 Voice Navigation

Allow visitors to navigate your website naturally.

Examples:

```text
"Open Pricing"
→ /pricing

"Go to Contact"
→ /contact

"Show Services"
→ /services
```

---

## ⚡ Easy Website Integration

Embed the assistant into **any website** with a single script.

No React.

No framework.

Works with any website.

---

## 💳 Subscription Plans

* Free Plan
* Pro Plan
* Monthly Usage Limits
* Razorpay Checkout
* 90-Day Pro Subscription

---

## 🎨 Dashboard

* Responsive Design
* Tailwind CSS
* Live Assistant Preview
* Toast Notifications
* Protected Routes

---

# 🛠 Tech Stack

## Frontend

* React
* Tailwind CSS

---

## Backend

* Node.js
* Express.js
* MongoDB
* Mongoose

---

## AI

* Google Gemini API

---

## Payments

* Razorpay

---

## Widget

* Vanilla JavaScript
* Vanilla CSS
* Framework Independent

---

# 📂 Project Structure

```text
AIVoiceAgent/
│
├── client/
│   ├── public/
│   │   ├── assistant.js
│   │   └── assistant.css
│   │
│   └── src/
│       ├── Components/
│       ├── pages/
│       ├── utils/
│       └── App.jsx
│
└── server/
    ├── Configs/
    ├── Controllers/
    ├── Middleware/
    ├── Models/
    ├── Routes/
    └── index.js
```

---

# 🚀 Getting Started

## Prerequisites

* Node.js 18+
* MongoDB Database
* Firebase Project
* Razorpay Account
* Google Gemini API Key

---

## 1. Clone Repository

```bash
git clone https://github.com/ArcSaber21/AIVoiceAgent.git

cd AIVoiceAgent
```

---

## 2. Server Setup

```bash
cd server

npm install
```

Create a `.env` file inside the **server** directory.

```env
PORT=5000
MONGODB_URL=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
RAZORPAY_KEY_ID=your_razorpay_key
RAZORPAY_KEY_SECRET=your_razorpay_secret
```

Start the server.

```bash
npm run dev
```

---

## 3. Client Setup

```bash
cd client

npm install
```

Create a `.env` file inside the **client** directory.

```env
VITE_FIREBASE_API_KEY=your_firebase_api_key
```

Run the client.

```bash
npm run dev
```

---

# 🌍 Embedding the Assistant

After creating and configuring your AI assistant from the dashboard, you'll receive your **User ID**.

Open your website's **`index.html`** file and paste the following code **inside the `<body>` tag, just above the closing `</body>` tag.**

```html
<body>

    <!-- Your Website Content -->

    <script
        src="https://wishai.onrender.com/assistant.js"
        data-user-id="YOUR_USER_ID">
    </script>

</body>
```

> **Important:** Place the script **immediately above the closing `</body>` tag**. This ensures the widget loads after the page content, improving performance and avoiding render blocking.

Once added, the assistant automatically loads your configuration and becomes available to your website visitors.

---

# 📡 API Endpoints

| Method | Endpoint                        | Description                          |
| ------ | ------------------------------- | ------------------------------------ |
| POST   | `/api/auth/google`              | Google Sign In / Register            |
| GET    | `/api/auth/logout`              | Logout                               |
| GET    | `/api/assistant/config/:userId` | Fetch Public Assistant Configuration |
| POST   | `/api/assistant/ask`            | Send Message to AI                   |
| POST   | `/api/billing/order`            | Create Razorpay Order                |
| POST   | `/api/billing/verify`           | Verify Payment & Upgrade to Pro      |

---

# 🔒 Security

* Firebase Authentication
* JWT Authentication
* HTTP-Only Cookies
* Protected API Routes
* Secure Razorpay Payment Verification

---

# 🚀 Future Improvements

* Streaming Voice Conversations
* Text-to-Speech Voices
* Conversation History
* Analytics Dashboard
* Custom Branding
* Multiple Assistants
* Team Collaboration
* Widget Position Customization
* Multi-language Support

---

# 🤝 Contributing

Contributions are welcome!

Feel free to fork the repository, open issues, or submit pull requests.

---

# ⭐ Support

If you found this project useful, consider giving it a **⭐ Star** on GitHub.

It helps others discover the project and motivates future development.

---

# 📄 License

No license has been added yet.

If you plan to make this project open source, consider using the **MIT License**.

---

<div align="center">

### Built with ❤️ using React, Node.js, MongoDB, Firebase & Google Gemini

</div>
