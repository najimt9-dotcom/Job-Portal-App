🚀 Tech Stack

Frontend

React / Vite

Tailwind CSS

Axios

Backend

Node.js

Express.js

MongoDB (Atlas)

Cloudinary (for media storage)

Clerk (Authentication)

Sentry (Optional – Error Tracking)

Deployment

Vercel (Backend & Frontend)

📦 Prerequisites

Before starting, make sure you have the following installed:

Node.js (Ignore if already installed)
👉 Download from: https://nodejs.org/en/download/

Git

VS Code

⚙️ Project Setup Guide

Important: Always run and deploy the Server first, then start the Client.

🖥️ Server Setup (Backend)
1. Open Project Folder

Open the backend project folder in VS Code.

2. Install Dependencies
npm install

3. Setup MongoDB

Create a MongoDB Atlas account
👉 https://www.mongodb.com/cloud/atlas/register

Create a cluster and obtain your MongoDB URI

Add it to your .env file:

MONGO_URI=your_mongodb_uri

4. Setup Cloudinary

Register at: https://cloudinary.com/users/register_free

Get Cloud Name, API Key, and API Secret

CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret

5. Setup Clerk (Authentication)

Register at: https://clerk.com/

Create an application

Get your Clerk keys

CLERK_SECRET_KEY=your_clerk_secret_key

6. Setup Sentry (Optional)

Register at: https://sentry.io/

Add DSN if required

7. Push Project to GitHub

Create a GitHub repository and push your backend code.

8. Deploy Backend on Vercel

Visit: https://vercel.com/

Import your backend repository

Deploy and obtain the Backend URL

9. Setup Clerk Webhook

Go to Clerk Dashboard
👉 https://dashboard.clerk.com/

Configure webhook using your deployed backend URL

Re-deploy backend after webhook setup

▶️ Run Server Locally
npm run dev


✅ Make sure the backend is running or deployed before starting the client.

💻 Client Setup (Frontend)
1. Open Client Folder

Open the frontend folder in VS Code Integrated Terminal.

2. Install Dependencies
npm install

3. Add Environment Variables

Create a .env file:

VITE_BACKEND_URL=your_backend_url
VITE_CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key

4. Run Client Project
npm run dev

🌐 Deployment (Client)

Deploy the frontend on Vercel

Add the environment variables in Vercel Dashboard

Redeploy the project

✅ Features

User Authentication (Clerk)

Job Posting & Management

Job Application System

Secure API Integration

Cloud Image Uploads

Error Monitoring (Sentry – Optional)

📌 Notes

Ensure backend is deployed and running before starting the client.

Double-check environment variables before deployment.

Webhooks must be correctly configured for Clerk authentication.
