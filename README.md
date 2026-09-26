\# Social Media Automation Platform



A full-stack social media automation and scheduling platform built with React, TypeScript, Node.js, and Express.



The application allows users to connect social media accounts, create posts, generate content with AI, upload media, schedule posts, and automatically publish scheduled content to connected platforms.



\## ✨ Features



\- 🔐 User authentication

\- 🔗 Connect and manage social media accounts

\- ✍️ Create and schedule social media posts

\- 🤖 AI-powered content generation

\- 🎨 Multiple AI writing tones

\- 🖼️ AI image generation support

\- 📤 Image and media uploads

\- 📅 Schedule posts for a specific date and time

\- 🚀 Automatic scheduled publishing

\- 📊 Dashboard and activity tracking

\- 📝 Post generation history

\- 🔄 Automatic scheduler service

\- ☁️ Cloudinary media storage

\- 🔌 Social media publishing through Zernio



\## 🏗️ Project Structure



```text

social-scheduler/

│

├── client/                 # React frontend

│   ├── public/

│   ├── src/

│   │   ├── api/

│   │   ├── assets/

│   │   ├── components/

│   │   ├── context/

│   │   └── pages/

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

🛠️ Tech Stack

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

JWT Authentication

bcrypt

Multer

node-cron

External Services

Google Gemini / Google GenAI

Cloudinary

Zernio

MongoDB

🚀 Getting Started

Prerequisites



Make sure you have the following installed:



Node.js

npm

MongoDB

Git



Clone the repository:



git clone https://github.com/Vishwas-Arora/social-media-automation.git



Move into the project:



cd social-media-automation

📦 Install Dependencies

Client



Open a terminal in the client directory:



cd client

npm install

Server



Open another terminal and run:



cd server

npm install

🔐 Environment Variables



Environment variables are required for the application to work correctly.



Create:



client/.env

server/.env



Do not commit these files to GitHub.



Server Environment Variables



The exact variables depend on the services configured for your deployment. Typical configuration includes:



PORT=5000

MONGODB\_URI=your\_mongodb\_connection\_string

JWT\_SECRET=your\_jwt\_secret



CLOUDINARY\_CLOUD\_NAME=your\_cloudinary\_cloud\_name

CLOUDINARY\_API\_KEY=your\_cloudinary\_api\_key

CLOUDINARY\_API\_SECRET=your\_cloudinary\_api\_secret



ZERNIO\_API\_KEY=your\_zernio\_api\_key



GEMINI\_API\_KEY=your\_gemini\_api\_key

Client Environment Variables



Configure the frontend API URL according to your local or production backend.



Example:



VITE\_API\_URL=http://localhost:5000



Never publish real API keys, passwords, JWT secrets, or database credentials.



▶️ Running the Application

Start the Backend



From the server directory:



npm run server



The development server uses nodemon and tsx.



Start the Frontend



From the client directory:



npm run dev



Vite will provide a local development URL in the terminal.



Open that URL in your browser.



🧠 AI Content Generation



The platform includes an AI Composer that can generate social media content from a user prompt.



Users can select different writing styles such as:



Professional

Creative

Funny

Minimalist

Excited



Generated content can then be scheduled for publication.



📅 Social Media Scheduling



Users can:



Create a post

Select one or more social platforms

Add text content

Upload media when required

Select a date

Select a time

Schedule the post



The backend scheduler checks for posts that are due and processes them automatically.



🚀 Automated Publishing



The backend uses a scheduled job to check for posts that are ready to be published.



When a scheduled post reaches its publication time, the application:



Finds the user's connected social accounts

Builds the publishing payload

Sends the post to the configured publishing service

Updates the post status

Records the publishing activity

📁 Important Notes

Environment Files



.env files are intentionally excluded from Git using .gitignore.



Never commit credentials or secrets to the repository.



Dependencies



node\_modules directories are also excluded from Git.



Install dependencies with:



npm install



instead of committing node\_modules.



🔧 Available Scripts

Client



Development:



npm run dev



Production build:



npm run build



Lint:



npm run lint



Preview production build:



npm run preview

Server



Development:



npm run server



Production/start:



npm start



Build:



npm run build

🔄 Updating the Repository



After making changes:



git add .

git commit -m "Describe your changes"

git push



Example:



git add .

git commit -m "Added post scheduling improvements"

git push

📌 Project Status



This project is currently under development.



Features and integrations may change as the application evolves.



📄 License



No open-source license has currently been specified for this project.





\### Add it to GitHub



Since you're already using Git Bash, this is easiest.



Go to your project folder:



```bash

cd \~/Downloads/Social-Media-Automation-Project-Source-Code/social-scheduler

