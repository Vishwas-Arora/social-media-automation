# Social Media Automation Platform

A full-stack application for creating, managing, scheduling, and publishing social media content from one place.

The project has a React frontend and a Node.js/Express backend, with AI-assisted content generation and integrations for media storage and social media publishing.

## Features

- User authentication
- Social media account management
- Create and schedule posts
- AI-assisted content generation
- Multiple content writing styles
- AI image generation
- Image and media uploads
- Scheduled post publishing
- Dashboard and activity tracking
- Post generation history
- Automated scheduling service
- Cloudinary media storage
- Zernio integration for social media publishing

## Project Structure

```text
social-scheduler/
├── client/                 # React frontend
│   ├── public/
│   ├── src/
│   ├── package.json
│   └── vite.config.ts
│
├── server/                 # Node.js / Express backend
│   ├── config/
│   ├── controllers/
│   ├── middlewares/
│   ├── models/
│   ├── routes/
│   ├── services/
│   ├── package.json
│   └── server.ts
│
├── .gitignore
└── How to Run Project.pdf
Tech Stack
Frontend
React
TypeScript
Vite
Tailwind CSS
React Router
Axios
Lucide React
React Hot Toast
Backend
Node.js
Express
TypeScript
MongoDB
Mongoose
JWT
bcrypt
Multer
node-cron
Services
Google Gemini / Google GenAI
Cloudinary
Zernio
MongoDB
Getting Started
Prerequisites

Make sure you have these installed:

Node.js
npm
MongoDB
Git
Clone the repository
git clone https://github.com/Vishwas-Arora/social-media-automation.git
cd social-media-automation
Installation

Install the frontend dependencies:

cd client
npm install

Install the backend dependencies:

cd ../server
npm install
Environment Variables

The application uses environment variables for configuration and API credentials.

Create the following files locally:

client/.env
server/.env

These files are excluded from Git using .gitignore.

Server

Configure the required backend variables in server/.env.

For example:

PORT=5000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret

CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_API_SECRET=your_cloudinary_api_secret

ZERNIO_API_KEY=your_zernio_api_key
GEMINI_API_KEY=your_gemini_api_key
Client

Configure the frontend API URL in client/.env:

VITE_API_URL=http://localhost:5000

Never commit API keys, passwords, database credentials, JWT secrets, or other sensitive information to GitHub.

Running the Application
Start the backend

From the server directory:

npm run server
Start the frontend

From the client directory:

npm run dev

Vite will display the local development URL in the terminal.

AI Content Generation

The application includes an AI content composer that can generate social media content from a user's prompt.

Users can choose different writing styles, such as:

Professional
Creative
Funny
Minimalist
Excited

The generated content can then be edited and scheduled for publishing.

Post Scheduling

Users can:

Create a post
Select social media accounts
Add text content
Upload media
Select a date and time
Schedule the post

The backend scheduler periodically checks for posts that are ready to be published.

Automated Publishing

When a scheduled post reaches its publishing time, the backend processes the post and sends it to the configured social media publishing service.

The application then updates the post status and records the related activity.

Security

The project uses a .gitignore file to prevent sensitive files such as .env and dependency directories such as node_modules from being committed.

Do not expose production credentials or API keys in the source code.

Updating the Project

After making changes to the project:

git add .
git commit -m "Describe your changes"
git push

For example:

git add .
git commit -m "Improve post scheduling"
git push
Project Status

This project is currently under development.

Features, integrations, and configuration may change as development continues.

#License

No open-source license has currently been specified for this project.
