# Real-Time Chat Application

A modern, real-time chat application built with React, Node.js, Socket.IO, and MongoDB.

## 🚀 Features

- **Real-time messaging** with Socket.IO
- **User authentication** with JWT
- **Image uploads** via Cloudinary
- **Responsive design** with DaisyUI
- **Online user status** tracking
- **Modern UI/UX** with React and Vite

## 🛠️ Tech Stack

### Frontend
- **React 18** - UI framework
- **Vite** - Build tool and dev server
- **DaisyUI** - CSS framework
- **Zustand** - State management
- **Socket.IO Client** - Real-time communication
- **Axios** - HTTP client
- **React Router** - Navigation
- **React Hot Toast** - Notifications

### Backend
- **Node.js** - Runtime environment
- **Express.js** - Web framework
- **Socket.IO** - Real-time communication
- **MongoDB** - Database
- **Mongoose** - ODM
- **JWT** - Authentication
- **bcryptjs** - Password hashing
- **Cloudinary** - Image storage
- **CORS** - Cross-origin resource sharing

## 📦 Installation

### Prerequisites
- Node.js (v16 or higher)
- MongoDB Atlas account
- Cloudinary account

### Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/Tejaswini7396/RealTimeChatapp.git
   cd RealTimeChatapp
   ```

2. **Install dependencies**
   ```bash
   # Install backend dependencies
   cd ChatApp/backend
   npm install

   # Install frontend dependencies
   cd ../frontend
   npm install
   ```

3. **Environment Variables**

   Create a `.env` file in `ChatApp/backend/`:
   ```env
   MONGODB_URI=your_mongodb_connection_string
   PORT=3001
   JWT_SECRET=your_jwt_secret
   NODE_ENV=development
   CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
   CLOUDINARY_API_KEY=your_cloudinary_api_key
   CLOUDINARY_API_SECRET=your_cloudinary_api_secret
   ```

4. **Run the application**
   ```bash
   # Start backend (from ChatApp/backend)
   npm run dev

   # Start frontend (from ChatApp/frontend)
   npm run dev
   ```

## 🌐 Usage

1. Open your browser and go to `http://localhost:5173`
2. Create a new account or sign in
3. Start chatting in real-time!

## 📁 Project Structure

```
ChatApp/
├── backend/
│   ├── src/
│   │   ├── controllers/
│   │   ├── lib/
│   │   ├── middleware/
│   │   ├── models/
│   │   ├── routes/
│   │   └── index.js
│   ├── package.json
│   └── .env
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── store/
│   │   ├── lib/
│   │   └── main.jsx
│   ├── package.json
│   └── index.html
└── README.md
```

## 🔧 Configuration

### MongoDB Atlas Setup
1. Create a MongoDB Atlas account
2. Create a new cluster
3. Get your connection string
4. Add database name to connection string: `mongodb+srv://.../realtimechat?retryWrites=true&w=majority`

### Cloudinary Setup
1. Create a Cloudinary account
2. Get your cloud name, API key, and API secret
3. Add them to your `.env` file

## 🚀 Deployment

### Backend Deployment
- Deploy to platforms like Heroku, Railway, or Render
- Set environment variables in your hosting platform
- Update CORS settings for production

### Frontend Deployment
- Build the project: `npm run build`
- Deploy to Vercel, Netlify, or similar platforms
- Update API endpoints for production

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 👨‍💻 Author

**Tejaswini** - [GitHub](https://github.com/Tejaswini7396)

---

⭐ Star this repository if you found it helpful! 