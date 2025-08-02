# Deploy to Render

## Step-by-Step Deployment Guide

### 1. Prepare Your Repository
Your repository is already configured for Render deployment with:
- `render.yaml` - Render configuration
- Updated `package.json` scripts
- Production-ready backend and frontend

### 2. Deploy on Render

1. **Go to [Render.com](https://render.com)** and sign up/login

2. **Connect Your GitHub Repository**
   - Click "New +" → "Web Service"
   - Connect your GitHub account
   - Select your repository: `Tejaswini7396/RealTimeChatapp`

3. **Configure the Service**
   - **Name**: `realtime-chat-app`
   - **Environment**: `Node`
   - **Region**: Choose closest to you
   - **Branch**: `master`
   - **Root Directory**: `ChatApp`
   - **Build Command**: `npm run install:all && npm run build`
   - **Start Command**: `npm run start:prod`

4. **Set Environment Variables**
   Click "Environment" tab and add:
   ```
   NODE_ENV=production
   PORT=10000
   MONGODB_URI=your_mongodb_atlas_connection_string
   JWT_SECRET=your_jwt_secret
   CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
   CLOUDINARY_API_KEY=your_cloudinary_api_key
   CLOUDINARY_API_SECRET=your_cloudinary_api_secret
   CLIENT_URL=https://your-app-name.onrender.com
   ```

5. **Deploy**
   - Click "Create Web Service"
   - Render will automatically build and deploy your app

### 3. Your App Will Be Available At:
`https://your-app-name.onrender.com`

### 4. Features After Deployment:
- ✅ Full-stack application on one URL
- ✅ Real-time messaging with Socket.IO
- ✅ User authentication
- ✅ Image uploads via Cloudinary
- ✅ MongoDB Atlas database
- ✅ Automatic HTTPS
- ✅ Free tier available

### 5. Troubleshooting:
- Check Render logs if deployment fails
- Ensure all environment variables are set
- Verify MongoDB Atlas connection
- Check Cloudinary credentials

## Alternative: Railway Deployment

If you prefer Railway:
1. Go to [Railway.app](https://railway.app)
2. Connect your GitHub repository
3. Railway will auto-detect the configuration
4. Set environment variables
5. Deploy!

Your app will work on both platforms! 🚀 